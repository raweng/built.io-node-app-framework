##built.io Application Framework for NodeJS
<br/>
A framework thats built on top of Express Framework  and it helps the javascript developers to start developing javascript application using node js on the server side.

Basic features provided by  this framework is as follows:

-    Organize the code in well defined directory structure and implies some convention to be follow at the time of development
-    Helps to utilize the CPU core based on configurable value.
-    Forever-monitor module integrated in framework for making sure application run for forever
-	**Proxy Module** : It helps to proxy the request and provide the way to intercept the request before the proxy call is made . It provides three types of hooks for the request
    -	**before**:  Can intercept the proxy call and allows to change the request parameters and headers.  
    -	**after**: Its an async hook and fires when the request is completed
    -	**error**: Its an async hook and fires when error occurred in the request
-	**Log Module**: It provide two types of logging
    -	**User Log**: It logs all the console.log  statements in the user_log{stamp}.LOG file located in log directory. Developers can turn it on/off based on the configuration.
    - **Error Log**: It logs all the error occured in application in the error_log{stamp}.LOG file located in log directory.
-	**Routes/Resource**: It help to define the routes/resource of an application in route.json file located in config directory.
-	**Environment Configs**:  It helps to defined different environment configuration and load accordingly.

<br/>

###Directory Structure:

To create an application developer has to only deal with app directory located in application root.

<table border="1">
 <tr>
  <td>
  <center><b>Dir/Files</b></center>
  </td>
  <td>
  <center><b>Purpose</b></center>
  </td>
 </tr>
 <tr>
  <td>
  app/
  </td>
  <td>
  Contains client and server directory
  </td>
 </tr>
 <tr>
  <td >
  app/client
  </td>
  <td>
  Contains all client side files
  publically accessible like JS, CSS, IMAGES 
  </td>
 </tr>
 <tr >
  <td >
  app/server
  </td>
  <td >
  Contains all server side files
  </td>
 </tr>
 <tr >
  <td >
 app/server/config
  </td>
  <td>
  Contains configuration files
  </td>
 </tr>
 <tr>
  <td>
 app/server/config/environment
  </td>
  <td>
 Contains development and production configuration files
  </td>
 </tr>
 <tr>
  <td>
 app/server/config/environment/development.json
  </td>
  <td>
  Contains application configuration for development mode
  </td>
 </tr>
 <tr>
  <td>
 app/server/config/environment/production.json
  </td>
  <td>
  Contains application configuration for production mode
  </td>
 </tr>
 <tr>
  <td>
  app/server/config/app_events.json
  </td>
  <td>
  Contains hooks for application events
  like init, error etc.
  </td>
 </tr>
 <tr>
  <td>
  app/server/config/proxy.json
  </td>
  <td>
  Contains proxy routes
  </td>
 </tr>
 <tr>
  <td>
  app/server/config/route.json
  </td>
  <td>
  Contains all routes and resources of an application
  </td>
 </tr>
 <tr>
  <td>
  app/server/controllers
  </td>
  <td >
  Contains all controllers of an application
  </td>
 </tr>
 <tr >
  <td>
  app/server/files
  </td>
  <td>
  File uploaded via client automatically available in this directory
  </td>
 </tr>
 <tr>
  <td >
  app/server/node_modules
  </td>
  <td>
  Contains Third party node modules required for an application
  </td>
 </tr>
 <tr>
  <td>
  app/server/templates
  </td>
  <td>
  Contains application templates
  </td>
 </tr>
 <tr>
  <td>
  app/server/package.json
  </td>
  <td>
  Contains all configuration of an application
  </td>
 </tr>
 <tr>
  <td>
  app/log
  </td>
  <td>
  Contains application log files
  </td>
 </tr>
</table>
