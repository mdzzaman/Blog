# JMeter
The Apache JMeter™ application is open source software, a 100% pure Java application designed to load test functional behavior and measure performance. It was originally designed for testing Web Applications but has since expanded to other test functions.

## Install
1. Install Java
    - Because JMeter is pure Java desktop application, it requires a fully compliant JVM 6 or higher. You can download and install the latest version of **Java SE Development Kit**. [Download Java Platform (JDK)](https://www.oracle.com/java/technologies/javase-downloads.html). [_Download_](https://download.oracle.com/java/18/latest/jdk-18_windows-x64_bin.exe)
1. Download JMeter
    - [Download Latest JMeter](https://jmeter.apache.org/download_jmeter.cgi) Choose the Binaries file (either zip or tgz) to download as shown in the figure below.
    ![Image](Asset/JMeter-Download.png)
    -Extract this .zip file
1. Run JMeter
    - Run this file `apache-jmeter-5.5\bin\jmeter.bat` from Extract folder then _JMeter_ will open.
    ![JMeterGUI](Asset/JMeter-GUI-info.png)

## Example
### Hello World
![](Asset/HelloWorld.gif)

https://www.youtube.com/watch?v=T-bTll7IRL0

## Set User Defined Variables
![](Asset/User_Defined_Variables.png)
Use This variable by `${variable}` in other place, like **HTTP Header Manager**, **HTTP Cookie Manager** etc.

## HTTP Header Manager
![](Asset/http-header-manager.png)
![](Asset/http-header-manager-2.png)

## HTTP Cookie Manager
![](Asset/http-cookie-manager.png)
![](Asset/http-cookie-manager-2.png)
### HTTP Cookie for all request and set automatically
we can use it in thread level
![](Asset/http-cookie-manager-3.png)
![](Asset/http-cookie-manager-4.png)

## JSON Extractor (Get access token)
![](Asset/json-extractor.png)
Then add **User Defined Variables**  *Token*
![](Asset/json-extractor-2.png)

## JSR223 PostProcessor (**!Important**)
- It will run after all redirect done

## Assertions
|TYPE | USAGE|
|-----|------|
|Response Assertion |	Apply a string pattern to verify against the server response|
|Duration Assertion |	Check the response was received within a given elapsed time|
|Size Assertion |	Check the size of the server response contains the wanted number of bytes|
|XML Assertion |	Check the response is a valid XML document|
|Beanshell Assertion |	Execute your own logic using Beanshell scripting|
|MD5Hex Assertion |	Allows to check the MD5 hash of the response data (great for static files)|
|HTML Assertion |	Check html response syntax using JTidy|
|XPath Assertion |	Tests if a document is well-formed, with possible DTD validation, or putting the document through JTidy and testing with XPath |
|XML Shema Assertion |	Validate an XML response against an XML schema|
|JSR223 Assertion |	Run your own code logic using a JSR223 Script|
|Compare Assertion |	Compares results between themselves|
|SMIME Assertion |	Evaluate the sample results from the Mail Reader Sampler|
|JSON Assertion |	Execute JsonPath expressions and validate Json documents|

## Assertions Performance
|ASSERTION |	CPU/MEMORY USAGE |	NOTES|
|----------|---------------------|-------|
|Response Assertion |	Moderate |	Regular Expressions|
|Duration Assertion |	Low |	|
|Size Assertion |	Low |	|
|XML Assertion |	High |	Builds XML DOM Documents|
|Beanshell Assertion |	Variable |	Depends on the script logic|
|MD5Hex Assertion |	Low |	|
|HTML Assertion |	High |	Parses the HTML Response|
|XPath Assertion |	High |	Builds XML DOM Documents|
|XML Schema | Assertion |	High	Builds XML DOM Documents|
|JSR223 Assertion |	Variable |	Depends on the script logic|
|Compare Assertion |	High |	Parses responses and compares them|
|SMIME Assertion |	Moderate |	|
|Json Assertion |	High |	Parses the Json document|


## Data Extract
### BeanShell Preprocessor
![](Asset/BeanShell-Preprocessor.png)
### CSS Selector Extractor
![](Asset/CSS-Selector-Extractor.png)
- Select data from html by css selector
- Set Attribute for get value
- Set data in variable for future use

- Crete Multiple Selector for multiple value

### BeanShell PostProcessor
- Get value from User Defined Variables
![](Asset/BeanShell-PostProcessor.png)

### Response Assertion
![](Asset/ResponseAssertion.png)

### Thread Group
![](Asset/ThreadGroup.png)


[r1](https://octoperf.com/blog/2018/04/19/jmeter-assertions/#supported-assertions)