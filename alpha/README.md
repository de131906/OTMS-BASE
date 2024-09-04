# OTMS-ALPHA

This is the top-level container project for all projects subject to
change frequently

- otms-base
- otms-client
- otms-server
- otms-loggerbase
- otms-wsoxclient

Within POM of all these projects include:
```
<dependencyManagement>
    <dependencies>
        <dependency>
            <groupId>${project.groupId}</groupId>
            <artifactId>otms-root</artifactId>
            <version>${project.version}</version>
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