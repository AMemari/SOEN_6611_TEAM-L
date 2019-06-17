Metric 1(Statement Coverage), 2(Branch Coverage) and 4(McCabe Complexity) can be calculated by using a code coverage tool like JaCoCo.<br>
Process to measure the metrics:<br>
Step 1: Check if EclEmma plugin is installed in Eclipse. If not, go to Help-> Eclipse Marketplace-> Search for EclEmma-> Install->               Restart Eclipse<br> 
Step 2: Import the maven project to Eclipse. File-> Import -> Existing Maven projects.<br>
Step 3: Add JaCoCo dependency to pom file of the Maven porject.<br>
Step 4: Run the porject as Maven Install and wait for the JaCoCo report to be generated. Code coverage report is generated in HTML, XML           and CSV format.<br> 


