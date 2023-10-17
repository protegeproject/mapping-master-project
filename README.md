## Mapping Master Build Project

This project contains a Maven POM that builds Mapping Master-related components.
Currently it builds the [core Mapping Master](https://github.com/protegeproject/mapping-master.git) project, 
the [Mapping Master Itegration Tests](https://github.com/protegeproject/mapping-master-integration-tests.git) project,
and the [Cellfie Plugin](https://github.com/protegeproject/cellfie-plugin.git) project.

#### Building

To run the build process in this project, you must have the following items installed:

+ [Java 11](https://www.oracle.com/java/technologies/downloads/archive/)
+ A tool for checking out a [Git](http://git-scm.com/) repository
+ Apache's [Maven](http://maven.apache.org/index.html)

Create a suitable local directory and then clone the Mapping Master-related projects as follows:

    git clone https://github.com/protegeproject/mapping-master.git
    git clone https://github.com/protegeproject/mapping-master-integration-tests.git
    git clone https://github.com/protegeproject/cellfie-plugin.git
    git clone https://github.com/protegeproject/mapping-master-project.git

Change into the Mapping Master project directory:

    cd mapping-master-project

And then build everything with Maven:

    mvn clean install

The Mapping Master integration tests can take quite a while to run. You can skip them as follows:

    mvn -DskipTests=true clean install

Documentation for Mapping Master can be found [here](https://github.com/protegeproject/mapping-master/wiki).
Documentation for the Cellfie plugin can be found [here](https://github.com/protegeproject/cellfie-plugin/wiki).

