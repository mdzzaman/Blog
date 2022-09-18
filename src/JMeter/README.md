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
### HTTP Cookie for all request and automatically set
we can use it in thread level
![](Asset/http-cookie-manager-3.png)
![](Asset/http-cookie-manager-4.png)

## JSON Extractor (Get access token)
![](Asset/json-extractor.png)
Then add **User Defined Variables**  *Token*
![](Asset/json-extractor-2.png)