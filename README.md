CI-for-SAP-Java
===============

Continuous Integration framework for SAP Java projects

This project contains a list of ant scripts for setting up a CI framework and to help getting started with the development of SAP Java projects using CI. The project installs the necessary software, configures it and provides templates for SAP Portal (Java) projects (NW Portal 7.0x and CE 7.2).

The ant script executes the following actions
1. download the software
2. installs it
3. configures the stack

What gets downloaded?

For the server side:
- Redmine 2
- Sonar 3
- Jenkins
- MySQL 5 server
- MySQL 5 connectorJ
- SCM Manager
- jRuby 1.6.7
- Tomcat 7
- selenium 2
- OpenDJ
- Solr 3.5

For the client tools (development and CI ant tasks)
- Ant
- Ivy
- jMeter
- curl
- svnkit
- TestNG


After the install script run through the CI stack is ready to be used. For SAP Portal developers there are ant scripts available to help setting up a CI project:
1. Creates a SVN repository
2. Creates a Jenkins job
3. Creates the Redmine project
4. Confiugres the central build file that Jenkins will execute to
a) call Sonar
b) deploys the portal archive
c) execute unit tests with TestNG
d) executes functional tests with selenium and jMeter


Default installation:
Tomcat: http://localhost:9090

Sonar: http://localhost:9090/sonar

Jenkins: http://localhost:9090/jenkins

SCM Manager: http://localhost:9090/scm
User: scmadmin / scmadmin

Solr: http://localhost:9090/solr
Admin page: /solr/admin

OpenDJ: localhost, port 389
cn=Directory Manager
Password: ch4nge

users created in LDAP:
sonar / sonar
developer / developer
admin / admin
jenkins / jenkins
redmine / redmine
scm / scm

The user used for creating later the SAP Portal projects is the developer user.