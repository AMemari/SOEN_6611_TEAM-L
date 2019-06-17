Metric 1(Statement Coverage), 2(Branch Coverage) and 4(McCabe Complexity) can be calculated by using a code coverage tool like JaCoCo.<br>
Process to measure the metrics:<br>
Step 1: Check if EclEmma plugin is installed in Eclipse. If not, go to Help-> Eclipse Marketplace-> Search for EclEmma-> Install->               Restart Eclipse<br> 
Step 2: Import the maven project to Eclipse. File-> Import -> Existing Maven projects.<br>
Step 3: Add JaCoCo dependency to pom file of the Maven porject.<br>
Step 4: Run the porject as Maven Install and wait for the JaCoCo report to be generated. Code coverage report is generated in HTML, XML           and CSV format.<br> 

# JaCoCo dependency in pom file:<br>
<plugin><br>
<groupId>org.jacoco</groupId><br>
<artifactId>jacoco-maven-plugin</artifactId><br>
<version>0.8.4</version><br>
<executions><br>
<execution><br>
<id>prepare-agent</id><br>
<goals><br>
<goal>prepare-agent</goal><br>
</goals><br>
</execution><br>
<execution><br>
<id>post-unit-test</id><br>
<phase>test</phase><br>
<goals><br>
<goal>report</goal><br>
</goals><br>
<configuration><br>
<!--Sets the path to the file which contains the execution data.--><br>
<dataFile>target/jacoco.exec</dataFile><br>
<!--Sets the output directory for the code coverage report.--><br>
<outputDirectory>target/jacoco-ut</outputDirectory><br>
</configuration><br>
</execution><br>
</executions><br>
</plugin><br>

