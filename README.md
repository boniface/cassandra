# Apache Cassandra 4.0 Beta1 Docker Image

These files are for building Apache Cassandra 4.0 Beta docker containers. With this  beta version, there will
 be no new features or breaking API changes in future Beta or GA builds. 
  
  
There is no official container images for beta version yet and so do not use in production. This is for testing purposes only 
  
Notable features include 
 
1. Higher Availability with 5x Faster Streaming 
 
2. Incremental Repair Improvements 
 
3. Audit Logging 
 
4. Data Center Security Enhancements
 
5. Virtual tables 
 
6. Java 11 Support 


# Running the Container

Create a bash script with your chosen CONTAINER NAME and YOUR LOCAL FOLDER as show below:
```
#!/bin/bash
docker run  --name [CONTAINER NAME] \
   -v [ YOUR LOCAL FOLDER]:/var/lib/cassandra \
   -p 7000:7000 \
   -p 7001:7001 \
   -p 7199:7199 \
   -p 9042:9042 \
   -p 9160:9160 \
   -p 9404:9404 \
   -d bonifacekabaso/cassandra4:4.0-beta1
```
Then run your script 

```sh YOURSCRIPT.sh```
