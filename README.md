# Selenium Automation

I have created an automation suite containing two high level scenarios 
- Create an account
- Add an item to basket and perform checkout

Below are the contents of the zip folder
- Source file
- Chrome driver executable
- TestNG.xml file

## Tools and Technologies used
- Eclipse oxygen.3a
- Selenium Webdriver 3.11
- TestNG version 6.14.3
- Java 1.8
- Chrome Version 73.0.3683.103
- Chrome driver version 2.37

## How to run the test suite
Please find below instructions to run the test suite
- Download & unzip the folder and import the project in Eclipse
- Update the location of chrome driver executable in the source code 
  - Inside beforeSuite() method update line: System.setProperty("webdriver.chrome.driver","chrome driver location")
- Change the email-id to unique value for every execution in the source code
  - Inside signup() method: driver.findElement(By.xpath("//input[@id='email_create']")).sendKeys("unique email id")
- Open testng.xml file
  - Right click-> Run as-> Testng Suite
