# 0x000 - statement as follows
The following is for study and test purposes only and is not commercial. If possible, please support the original version.<br>
[portswigger.net Official web site](https://portswigger.net/)

# 0x001 - Project INFO
## A: burploader INFO
BurpSuite Activation for mpleased.com<br>
BurpLoader is compiled from JDK8.<br>
Support BurpSuite Version: V2020.2 ~ Latest Version.<br>
Activation Date: After 10000.<br>
BurpLoader Runtime:<br>
&nbsp;&nbsp;recommended as required by BrupSuite.

## B: BurpSuite Java Runtime
Java Version >= 11<br>
Using JDK 11 OR Higher.

## C: The first run requires BurpSuite to be started and activated using BurpLoader
Refer to Section 0x002 for BurpLoader and BurpSuite startup methods

# 0x002 - Startting Examples.
## A: Directory Structure
### a: Directory Structure A
```bash
BurpSuite_Pro_v2022.8.1
│  burpsuite_pro_v2022.8.1.jar
│  start_burpsuite_en_v2022.8.1.bat
│
├─Activation_Licenses
│  burploader_by_mpleased.com.jar
│  start_burploader_by_mpleased.com.bat
│
└─SoftwareEnvironment
    └─Java
       └─jdk-16.0.1
       
```
### b: Directory Structure B <-- Recommand 
```bash
BurpSuite_Pro_v2022.8.1
│  burpsuite_pro_v2022.8.1.jar
│  start_burpsuite_en_v2022.8.1.bat
│  burploader_by_mpleased.com.jar
|  start_burploader_by_mpleased.com.bat
|
└─SoftwareEnvironment
    └─Java
       └─jdk-16.0.1
       
```
## B: BurpLoader startting scripts for windows bat.
\# start_burploader_by_mpleased.com.bat
```powershell
@echo off
SET CPWD=%~dp0
rem Stting JAVA Environment Variables.
rem It corresponds to directory structure A
SET JAVA_HOME=%CPWD%..\SoftwareEnvironment\Java\jdk-16.0.1
rem It corresponds to directory structure B
rem SET JAVA_HOME=%CPWD%\SoftwareEnvironment\Java\jdk-16.0.1
SET PATH=%JAVA_HOME%\bin
SET CLASSPATH=.;%JAVA_HOME%\lib
START java -jar burploader_by_mpleased.jar pause exit
```
## C: Burpsuite startting scripts for windows bat.
\# start_burpsuite_en_v2022.8.1.bat
```powershell
@echo off
SET CPWD=%~dp0
rem Stting JAVA Environment Variables.
SET JAVA_HOME=%CPWD%\SoftwareEnvironment\Java\jdk-16.0.1
SET PATH=%JAVA_HOME%\bin
SET CLASSPATH=.;%JAVA_HOME%\lib
rem Core Startup Command.
START java --illegal-access=permit -javaagent:Activation_Licenses\burploader_by_mpleased.com.jar -Dfile.encoding=utf-8 -noverify -jar -Xmx3072M burpsuite_pro_v2020.8.1.jar pause exit
```
## D: Using burpload strartup BurpSuite.
\# Important: The following conditions must be met.<br>
\# A: Only if the current JDK version is able to launch BurpSuite directly.<br>
\# B: Burploader and BurpSuite are in the same directory.<br>
\# C: Install the Java environment ahead of time.<br>
1.Running The BurpLoader Jar File.<br>
```powershell
java -jar burploader_by_mpleased.com.jar
```
2.Click the Run Button Startup The BurpSuite<br>
3.Complete the activation process.
