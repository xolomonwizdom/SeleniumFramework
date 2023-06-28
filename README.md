# SeleniumFramework
This is a test framework that uses Selenium for browser automation and uses other dependencies:
1) TestNG - used for testing framework
2) Selenium API
3) Apache Commons
4) Jackson
5) Extent Reports
6) Maven
7) Maven profiling integration
8) Java

Setup for framework - uses Page Object Model for Design Pattern
1) Each page for the application has its class (pages package)

2) Utils package is used which has the following classes - 
i) ExtentReportHelper - used to create the extent report object (a single object is created and used for multiple test scenarios)
ii) ListenerHelper - uses ITestListener - which helps in creating the report as per different functions
iii) PropertyReaderHelper - helps to read the global config file

3) Base package is used which has the following classes - 
i) SetupDriver - This helps different drivers like chrome.firefox and edge which will trigger using the browserType key.
ii) CustomWaits - Converted thread.sleep into an easy-to-use function (can be used similarly for Explicit and Implicit wait)
iii) Commons - This is used to set up the Json data file for test scenarios

4) TestConfiguration package - BaseTest - used for setting up before and after functions.

5) TestData package - For setting up the json file which contains the testData

6) TestNG - Priority, description, dataProvider, and groups are covered
