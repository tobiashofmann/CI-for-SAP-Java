CI-for-SAP-Java
===============

Continuous Integration framework for SAP Java projects

This project contains a list of ant scripts for setting up a CI framework and to help getting started with the development of SAP Java projects using CI. The project installs the necessary software, configures it and provides templates for SAP Portal (Java) projects (NW Portal 7.0x and CE 7.2).

The ant script executes the following actions
1. download the software
2. installs it
3. configures the stack

Afterwards, the CI stack is ready to be used. For SAP Portal developers the ant scripts available help setting up a CI project:
1. Creates a SVN repository
2. Creates a Jenkins job
3. Creates the Redmine project
4. Confiugres the central build file that Jenkins will execute to
a) call Sonar
b) deploys the portal archive
c) execute unit tests with TestNG
d) executes functional tests with selenium and jMeter