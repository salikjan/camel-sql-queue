# camel-sql-queue
Route message from ActiveMQ to Derby Database using Camel
---

1. Dependencies for Apache ServiceMix

feature:repo-add camel 2.16.4
feature:install camel

feature:install camel-spring
feature:install camel-sql

feature:install spring-jdbc

bundle:install -s mvn:commons-dbcp/commons-dbcp/1.4
bundle:install -s mvn:commons-dbcp/commons-dbcp/1.6
bundle:install -s mvn:org.apache.derby/derby/10.12.1.1

2. To build this project use
   mvn install
   
3. To deploy the project in Apache Servicemix run the following command
   bundle:install -s mvn:ru.sydev/message_reader/1.0.0-SNAPSHOT

4. You can also run this project by
   mvn camel:run

