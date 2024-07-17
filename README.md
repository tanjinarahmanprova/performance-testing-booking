
# Performance Testing


## Table of content
- [Overview](#overview)
- [Prerequisites](#prerequisites)
- [Installation and Setup](#installation-and-setup)
    - [Java JDK](#java-jdk)
    - [Apache JMeter](#apache-jmeter)
    
- [Project Installation Steps](#project-installation-steps)
- [Description of Project](#description-of-project)
    - [Test Plan](#test-plan)
    - [Collection of API](#collection-of-api)
    - [Test Execution and Report Generation](#test-execution-and-report-generation)
    - [Report of the project](#report-of-the-project)
- [Contact](#contact)

## Overview
This repository demonstrates Performance testing using Apache JMeter.


## Prerequisites
- [Java JDK](https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html)
- [Apache JMeter](https://jmeter.apache.org/download_jmeter.cgi)



## Installation and Setup
### java JDK
- Download the installer from the [Oracle Java SE Downloads](https://www.oracle.com/java/technologies/javase/jdk11-archive-downloads.html) page.
- Run the installer and set up the JDK.
- Set up JAVA_HOME and PATH environment variables:
    - Open System Properties.
    - Navigate to Environment Variables.
    - Add JAVA_HOME with the JDK installation path.
    - Update the PATH variable to include %JAVA_HOME%\bin.
- Verify Java installation by running java --version in a terminal.
### Apache JMeter
- Download binary file from [Apache JMeter's website](https://jmeter.apache.org/download_jmeter.cgi).
- Extract the file to a suitable location on computer.
- Set up PATH environment variables:
    - Open System Properties.
    - Navigate to Environment Variables.
    - Add the path to the bin directory of JMeter installation.
- Double-click on the jmeter.bat file of bin directory to start JMeter.


## Project Installation Steps
Follow these steps to set up and start using the framework

- [Fork](https://github.com/tanjinarahmanprova/performance-testing-booking.git) the repository.
- Clone
```
git https://github.com/tanjinarahmanprova/performance-testing-booking.git
```
- Launch Apache JMeter.
- Open the JMX File.
- Make any desired changes or additions to the project.

## Description of Project
### Test Plan
- Add Thread Group: Testplan > Add > Threads (Users) > Thread Group
- Configure the Thread Group:
    - Number of Threads (Users): This represents the number of virtual users you want to simulate.
    - Ramp-Up Period (in seconds): This is the time JMeter will take to start all the threads.
    - Loop Count: The number of times to execute the test.

![tp](https://github.com/user-attachments/assets/7536ce43-32e8-47ee-a853-c1816bb66103)
### Collection of API
- Create HTTP Request for frequently used API: Thread Group > Add > Sampler > HTTP Request.
- Save JMX File.
### Test Execution and Report Generation
- Make a report folder in the bin folder.
- Run Command in jmeter\bin folder.
- Generate JTL file.
    - -n: Run JMeter in non-GUI mode.
    - -t: Path to the JMeter test plan file.
    - -l: Path to save the results in a JTL file.
```
jmeter -n -t practice_800.jmx -l practice_800.jtl
```
(report\practice_800.jtl).   
- Generate HTML Report.
    - -g: Indicates that JMeter should generate a report from the specified JTL file.
    - -o: Specifies the output directory where the HTML report should be generated.
```
jmeter -g practice_800.jtl -o report\practice_800.html
```

### Report of the project
**Number of Threads 800 ; Ramp-Up Period 10s; Loop Count 1**

![r1](https://github.com/user-attachments/assets/03fbc2fd-6bdd-4dd6-a519-52a8f9be771e)
![r2](https://github.com/user-attachments/assets/4342f076-91b5-437c-a95f-d627a4838c00)

**Number of Threads 1000 ; Ramp-Up Period 10s; Loop Count 1**

![r3](https://github.com/user-attachments/assets/d8b4160f-143c-441d-a13a-94314194b3dc)
![r4](https://github.com/user-attachments/assets/a0ce864e-d3c6-4120-8980-870694a5dc6c)

**Number of Threads 1200 ; Ramp-Up Period 10s; Loop Count 1**

![r5](https://github.com/user-attachments/assets/24e3502d-8d4a-408b-9a75-894bee80df28)
![r6](https://github.com/user-attachments/assets/24e81f7a-0ebd-4190-ba4d-8777b180eddf)
![r7](https://github.com/user-attachments/assets/ab143587-b42b-413c-b221-d11f99c6bf1b)

## Contact
For questions or feedback, please feel free to reach out:
- **GitHub**: [Tanjina Rahman](https://github.com/tanjinarahmanprova)
- **Email**: [rahmantanjina983@gmail.com](mailto:rahmantanjina983@gmail.com)
- **LinkedIn**: [Tanjina Rahman](https://www.linkedin.com/in/tanjina-rahman-a53662191/)


