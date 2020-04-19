# Doctrin Co-worker details Test
> Retrieves all names and titles from the Co-worker section of career page of Doctrin site using Selenium with Cucumber-TestNG Hybrid framework

[![java Version][java-image]][java-url]
[![mvn Version][mvn-image]][mvn-url]
[![cucumber Version][cucumber-image]][cucumber-url]
[![testng Version][testng-image]][testng-url]
[![poi Version][poi-image]][poi-url]
[![sele Version][sele-image]][sele-url]
[![log Version][log-image]][log-url]

This test opens the career page of Doctrin site and retrieves all the names and titles from the co-worker section and creates a excel with all the details. This is wrapped around with by a library and framework build in java and maven to make writing tests, building and integrating with CI/CD systems easy. Cucumber-TestNG frameworks are also used. Cucumber makes test cases easy to maintain, create, read and understand to non-technical users while testNG is used to run the cucumber feature file and also makes it easy to integrate and scale with other systems.

![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/doctrincoworkerspagecloseup.png)

## Installation

OS X & Linux:

Install Brew

```sh
/bin/bash -c "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install.sh)"
```
Install Java

```sh
brew install java
```
Install Maven

```sh
brew install maven
```
Windows:

Follow the steps to install Java and Maven: [Link](https://howtodoinjava.com/maven/how-to-install-maven-on-windows/)

## Usage example

To run the test from terminal
```sh
mvn test
```
To clean files and directories generated by maven before the running the tests
```sh
mvn clean test
```

To change the Browser, open the ["DoctrinTitleListTest.feature"](/src/test/resources/DoctrinTitleListTest.feature) cucumber file in any editor and enter the desiered Browser name FF/Chrome and Version(Chrome versions:80,81,83 are supported).
Below is an example for the Browser FF with version 75.
![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/Cucumberfeature.png)

Note: The tests run in the background, give it time to finish and generate the report.

## Reporting

A Excel file report with the result of the run is created after each test run 
The Excel report file is located in 'ExcelReport' folder once the test has completed: [DoctrinTitleList/ExcelReport/CoworkerNameTitle.xls](/ExcelReport/)
![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/ExcelReport.png)

A log file also records details on the all the steps that are carried out and returns information in .log and .html formats. Its located in a folder called "DoctrinTitleList/log" created after runtime.
![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/log4jlog.png)
![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/log4jhtml.png)

A Cucumber report is generated after each test run.

The report is located in target folder once the test has completed: DoctrinTitleList/target/cucumber-html-report/cucumber-html-reports/overview-features.html

The overview-features.html is the report overview
![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/reportoverview.png)
The report-feature_DoctrinTitleListTest-feature.html can be accessed by clicking on the Feature name in the report overview. This shows all the test scenarios and test steps that are run as part of the test and also shows fail cases along with appropriate errors.
![](https://github.com/Rohan-Ganapathy/doctrinimages/blob/master/DoctrinTitleList/reportoverviewfeature.png)

## Meta

Author – [@RohanGanapathy](rohanganapathy@gmail.com)

[github](https://github.com/Rohan-Ganapathy)

<!-- Markdown link & img dfn's -->
[java-image]: https://img.shields.io/badge/java-1.7-orange
[java-url]: https://www.oracle.com/java/technologies/javase-jdk13-downloads.html
[mvn-image]: https://img.shields.io/badge/mvn-3.6.3-yellow
[mvn-url]: https://github.com/apache/maven
[cucumber-image]: https://img.shields.io/badge/cucumber-green
[cucumber-url]: https://github.com/cucumber/cucumber-jvm
[testng-image]: https://img.shields.io/badge/testng-darkgreen
[testng-url]: https://github.com/cucumber/cucumber-jvm/tree/master/testng
[poi-image]: https://img.shields.io/badge/apachepoi-blue
[poi-url]: https://github.com/apache/poi
[sele-image]: https://img.shields.io/badge/selenium-3.141.59-brightgreen
[sele-url]: https://github.com/apache/poi
[log-image]: https://img.shields.io/badge/log4j-darkorange
[log-url]: https://github.com/apache/log4j