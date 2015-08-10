# vlogging
Vnext Logging with NLog

Work sample from nuget package.

For Start with new project

 // Step 1. Create configuration object
 var config = new XmlLoggingConfiguration(Configuration.Get("DNX_APPBASE")+ "\\NLog.config");
 
 //add to source nuget 'https://www.myget.org/F/aspnetvnext/'
 //add Microsoft.Framework.Logging.NLog to project.json
 var fact = new NLog.LogFactory(config);
 loggerFactory.AddNLog(fact);
