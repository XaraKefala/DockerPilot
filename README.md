# DockerPilot

Welcome to DockerPilot, a container management application which seamlessly integrates the Docker Engine for   easy access and management of your Docker Cluster. 

With our app, you can effortlessly run and stop your Docker Containers, create new ones and inspect all the locally available Docker Containers and Images. Additionally, you have the ability capture the state of your Docker Cluster at any moment, automatically storing it into a local database to be accessed later. In this way, you can ensure that all the information is saved for future reference to be viewed and analyzed at your convenience, providing valuable insights into the historical state of the Docker environment.

## How to get and run the application

You will first need to clone this repository or download all the repository files to your computer. With [Java 8](https://www.java.com/download/ie_manual.jsp) and [Apache Maven](https://maven.apache.org/download.cgi) installed, go ahead and run `mvn install` on the command-line, while inside the folder of the application files.

After it is done compiling, packaging and installing the program, you can run the application from inside the newly created /target directory by running `java -jar DockerPilot-1.3.jar` on the command-line.

## How to use DockerPilot

Now that the application is up and running, you can explore various functionalities across three separate tabs: the Containers, Images and Container History tabs. Here is a brief overview of the actions available within each tab:
- The Containers Tab allows you to easily run, stop and inspect the selected containers (you can choose to view all the available containers or only the active or inactive ones) or add a new Measurement of the state of the Docker Cluster to the database.
- The Images Tab allows you to inspect all downloaded Images and create new Containers using them.
- The Container History tab allows you to select a specific Date and Measurement from the available entries of the database and view the state of the Docker environment at that specific moment via the corresponding Measurement.

## The Repository Architecture

- **.github/workflows:**  This directory contains **CI_Test.yml** file for continuous integration

- **src:** This is the first directory of the path that leads to code files (/src/main/java/gr/aueb/dmst
/ProjectPr/), images files usefull for the GUI (src/main/resources/images) and test files of the code (src/test/java/gr/aueb/dmst/ProjectPr)

- **pom.xml:** This file contains project information like dependencies and build configuration

- **sun_checks.xml:** This file is used for checking the format of the code 

## The UML Diagram of the program
![uml_final_transparent](https://github.com/XaraKefala/ProjectPr/assets/147168589/636de377-d8aa-4f59-84b3-12d46427a8bc)


## The Data Structures and Algorithms used in the code
**Data Structures:**
For the Database, we used SQLite. We save the data of the Docker Containers in two SQLite tables (Table Names: Measurment, DockerInstance) which store information like names, status, creation date of the containers and other data useful in the application.  

**Interfaces:**
- List
- Map
- Array

**Implementations:**
- ArrayList
- LinkedHashMap

## Creators
-**Kefala Charikleia Maria**
-**Korovesis Konstantinos Chrysovalantis**
-**Gounari Eleni**
-**Tsoukala Iliana**
-**Bratakos Andreas**
-**Manolaki Maria Dafni**
-**Agapaki Adamantia**
-**Poutios Aristotelis**


