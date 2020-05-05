# hola
hola microservice using Java EE (JAX-RS) on Microprofile/Thorntail

The detailed instructions to run *Red Hat Helloworld MSA* demo, can be found at the following repository: <https://github.com/redhat-helloworld-msa/helloworld-msa>


Build and Deploy hola locally
-----------------------------

1. Open a command prompt and navigate to the root directory of this microservice.
2. Type this command to build and execute the application:

        mvn wildfly-swarm:run

3. This will create a uber jar at  `target/hola-swarm.jar` and execute it.
4. The application will be running at the following URL: <http://localhost:8080/api/hola>

Deploy the application in Openshift
-----------------------------------

1. Make sure to be connected to the Openshift cluster
2. Execute

		mvn package fabric8:deploy
