# Lab-2
### Step 1
Run  command to create file structure:
#### mvn archetype:generate -DgroupId=com.example -DartifactId=my-app -DarchetypeArtifactId=maven-archetype-quickstart -DinteractiveMode=false! 

### Step 2
edit the file given file structure  (You can ignore the target folder it will generate it later) 
![Alt text](https://github.com/user-attachments/assets/620be773-a459-4f97-814a-fae16065cb9c)

### Step 3
Add the files from lab 1 that are made availible in said repo as a zip file. You can unzip them in the codespace with command unzip Lab.zip

### Step 4
Put all files that were in the c folder from lab 1 into the main/java folder. There should be a App.java file in the correct folder. **
![Alt text](https://github.com/user-attachments/assets/59d19192-c5f0-443c-b4dd-491a4ddabb67)


### Step 5
Now put the HybridTest.java from the u folder in Lab1 into the test/java folder. There should be a AppTest.java file there.
![Alt text](https://github.com/user-attachments/assets/9fe9335b-4fb6-44e9-b26b-f576ffbcb36d)

### Step 6
Put the Junit and Hamcrest files in to the resources folder you created when editing the file structure.

### Step 7
Outside the source folder there should be a file called pom.xml. open it and felace the code with said code. Changes are explained in report: 
```java
<project xmlns="http://maven.apache.org/POM/4.0.0"
         xmlns:xsi="http://www.w3.org/2001/XMLSchema-instance"
         xsi:schemaLocation="http://maven.apache.org/POM/4.0.0 http://maven.apache.org/xsd/maven-4.0.0.xsd">
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.companyname.bank</groupId>
    <artifactId>consumerBanking</artifactId>
    <version>1.0-SNAPSHOT</version>
    <packaging>jar</packaging>

    <properties>
        <maven.compiler.source>1.8</maven.compiler.source>
        <maven.compiler.target>1.8</maven.compiler.target>
        <maven.compiler.encoding>UTF-8</maven.compiler.encoding>
    </properties>

    <dependencies>
        <!-- JUnit 4.13.2 Dependency -->
        <dependency>
            <groupId>junit</groupId>
            <artifactId>junit</artifactId>
            <version>4.13.2</version>
            <scope>test</scope>
        </dependency>
    </dependencies>

    <build>
        <plugins>
            <!-- Surefire plugin to run the tests -->
            <plugin>
                <groupId>org.apache.maven.plugins</groupId>
                <artifactId>maven-surefire-plugin</artifactId>
                <version>2.22.2</version>
            </plugin>
        </plugins>
    </build>
</project>
```
### Step 8
To compile run command. 
```mvn compile```
Afterwards a new target folder is created with compiled code

### Step 9 
To run tests run command :
``` mvn clean test```
This will run the HybridTest.java file aswell as the default AppTest.java file. 





