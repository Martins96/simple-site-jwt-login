# Simple Site Jwt Login

## Description

This is the login part for simple site project, the module is divided in 2 parts:
 - BE microservice for login and signed JWT generation 
 - FE service, presentation layer, for interact to BE APIs
 
## Technologies
 
### Backend
The backend use Thorntail and Maven as core, for JWT generation the lib is Nimbus-Jose, REST APIs exposed via JAX-RS (RESTEasy Framework)
 
### Frontend
The frontend use Angular Framework as core

## Deployment
For deployment follow 2 step:
### Backend
Use `mvn clean package` for generate the full runnable JAR inside the target folder

### Frontend
Change the file **environment.prod.ts** adding the property *host* with the BE host endpoint
Use `ng build --prod` for build the FE application and generate the index.html + js files (deploy in a static HTML server)