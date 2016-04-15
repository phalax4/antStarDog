package com.app.core.utils;

import java.util.Date;
import org.apache.log4j.Logger;
//import org.apache.log4j.BasicConfigurator;
import java.io.*;
import java.util.*;
import java.io.FileInputStream;
import java.io.OutputStreamWriter;
import java.nio.file.Paths;

import com.complexible.common.openrdf.model.ModelIO;
import com.complexible.common.openrdf.model.Models2;
import com.complexible.common.rdf.model.Values;
import com.complexible.stardog.protocols.snarl.SNARLProtocolConstants;
import org.openrdf.model.IRI;
import org.openrdf.model.Model;
import org.openrdf.model.Resource;
import org.openrdf.model.vocabulary.RDF;
import org.openrdf.query.TupleQueryResult;
import org.openrdf.query.resultio.QueryResultIO;
import org.openrdf.rio.RDFFormat;

import com.complexible.common.protocols.server.Server;
import com.complexible.common.rdf.query.resultio.TextTableQueryResultWriter;
import com.complexible.stardog.Stardog;
import com.complexible.stardog.api.Connection;
import com.complexible.stardog.api.Getter;
import com.complexible.stardog.api.ConnectionConfiguration;
import com.complexible.stardog.api.SelectQuery;
import com.complexible.stardog.api.admin.AdminConnection;
import com.complexible.stardog.api.admin.AdminConnectionConfiguration;

import java.util.ArrayList;
import java.util.UUID;
import java.util.regex.Matcher;
import java.util.regex.Pattern;

import org.apache.jena.query.Query;
import org.apache.jena.query.QueryExecution;
import org.apache.jena.query.QueryExecutionFactory;
import org.apache.jena.query.QueryFactory;
import org.apache.jena.query.ResultSetFormatter;
public class DateUtils {
   static Logger log = Logger.getLogger(DateUtils.class.getName());
private Connection myConnection;
    //DatasetGraphNoSql datasetGraph = null;
    //private ResultSet rs = null;
    private String debug;
    private String nameSpace = "carnot:";
    private String nameSpacePrefix = "c";

	public static void main(String[] args) {
	
	try {
	AdminConnectionConfiguration dbmsConn = new AdminConnectionConfiguration();
			System.out.println("Configuration Done");
			AdminConnection dbmsAdminConn = dbmsConn.server("snarl://localhost:5820").credentials("admin", "admin").connect();
			
				System.out.println("Attempting Admin Connection");
				
				if(!dbmsAdminConn.list().contains("StarDogDB")){	//If DB doesnt already exist create it
					dbmsAdminConn.disk("StarDogDB").create(); // Still need to figure out where this file goes if embedded
				}
				System.out.println("Success");
			}catch(Exception e){	//Cannot Connect to External StardogDB
				//Build our embedded server
				System.out.println("Fatal");
			}
			
	
	
	
	
	
	
	
log.debug("Hello this is a debug message");
      log.info("Hello this is an info message");
    
		System.out.println(getLocalCurrentDate());
		
	}

	private static Date getLocalCurrentDate() {
		return new Date();		
	}

}
