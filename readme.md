# How to use robot-selenium project

## Create acceptance test cases

Create new test cases in "${project.basedir}/src/test/robotframework/acceptance" directory.

Create sub-directories in /acceptance, to group test cases.

All test cases should end with *.txt file extension.

## How to setup new web drivers

Setup is done by modifying the pom.xml

### Install new web drivers

Refer to https://github.com/webdriverextensions/webdriverextensions-maven-plugin, to install all the latest drivers or selectively install a particular driver and version, Chrome driver has been configured for example.

### Define the System Property for each web driver

Define driver in system properties, refer to https://seleniumhq.github.io/selenium/docs/api/java/constant-values.html.

Good way to identify what is the property name for each driver will be "webdriver.{browser}.driver"

Refer to the "properties-maven-plugin" configuration in pom.xml, Chrome driver has been configured for example.