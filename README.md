# OTMS-ROOT

This is the top-level container project.

## Maven Dependencies
Use this project as a Bill-Of-Material (BOM) ...
```
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>com.ibm.otms</groupId>
               <artifactId>otms-root</artifactId>
                <version>1.0-SNAPSHOT</version>
                <type>pom</type>
                <scope>import</scope>
            </dependency>
        </dependencies>
</dependencyManagement>
```
... and than import all required dependencies but omit the version tag
```
<dependency>
    <groupId>com.ibm.otms</groupId>
    <artifactId>otms-base</artifactId>
</dependency>
<dependency>
    <groupId>commons-logging</groupId>
	<artifactId>commons-logging</artifactId>
</dependency>
```
