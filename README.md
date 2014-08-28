Sample Demo App for Cloud Foundry OAuth
==============

Based on https://github.com/cloudfoundry/uaa

1. Execute the UAA WebApp:
```
mvn clean package tomcat7:run-war-only -PuaaWar
```
2. Execute the API Webapp:
```
mvn generate-resources tomcat7:run-war-only -PapiWar
```
3. Execute this sample WebApp:
```
mvn tomcat7:run-war-only
```
4. Open your browser on `http://localhost:10000/app`.

