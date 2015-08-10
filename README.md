# vlogging
Vnext Logging with NLog

Work sample from nuget package.

For Start with new project:

 Step 1. Add to source nuget 'https://www.myget.org/F/aspnetvnext/'
 
 Step 2. Add Microsoft.Framework.Logging.NLog to project.json
 
 Code:
 var config = new XmlLoggingConfiguration(Configuration.Get("DNX_APPBASE")+ "\\NLog.config");
 
 var fact = new NLog.LogFactory(config);
 
 loggerFactory.AddNLog(fact);
