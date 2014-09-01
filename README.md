Sample Demo App for Cloud Foundry OAuth
==============

Based on https://github.com/cloudfoundry/uaa

1. Go in the UAA directory: `cd be.sgerard.cloudfoundry.oauth.uaa`
2. Initialize the UAA database schema (only for the first time): `mvn generate-sources -Pdb-init,mysql`
3. Update the UAA database schema (only for the first time): `mvn generate-sources -Pdb-migrate,mysql`
4. Execute the UAA WebApp: `mvn clean package tomcat7:run-war-only -Pmysql`
5. Go in the API directory `cd be.sgerard.cloudfoundry.oauth.api`
6. Execute the API WebApp: `mvn clean package tomcat7:run-war-only`
7. Go in the sample WebApp: `cd be.sgerard.cloudfoundry.oauth.app`
8. Execute the sample WebApp: `mvn clean package tomcat7:run-war-only`
9. Open your browser on `http://localhost:10000/app`.

