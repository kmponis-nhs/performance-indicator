# Performance-Indicator
A java dependency to calculate execution time.

## Prerequisites
* To run the application you need to have git, mvn and JDK8 installed.

## Download
* Open command line and move to your workspace.
* Download project using your username: 
<br>`> git clone https://github.com/kmponis-nhs/performance-indicator.git`
* Go to project: 
<br>`> cd /performance-indicator`

## Run 
* Use terminal and move to your workspace
* Run in command line:
  <br>`> mvn clean install`

## Use
* Add to maven dependencies:
  <br>`<dependency>
    <groupId>com.sopra.steria</groupId>
    <artifactId>performance-indicator</artifactId>
    <version>0.0.1</version>
  </dependency>
  `

* Calculate performance by adding at the start and end of your block: 

  >Notes:<br>-Parameter 'your-name' for startTiming and endTiming methods should match.<br>-Default logging level is debug, to specify use "info", "warn" or "error".<br>-On endTiming method "description" is not mandatory, if null it will display nothing.

  **Logging level 'debug'**
    <br>`LogTimes.startTiming("your-name"); 
    LogTimes.endTiming("your-name"); 
      or 
    LogTimes.endTiming("your-name", "debug");
      or 
    LogTimes.endTiming("your-name", "debug", "your-description");  
    `
  **Logging level 'info'**
    <br>`LogTimes.startTiming("your-name"); 
    LogTimes.endTiming("your-name", "info");
      or 
    LogTimes.endTiming("your-name", "info", "your-description");
    `
  **Logging level 'warn'**
    <br>`LogTimes.startTiming("your-name"); 
    LogTimes.endTiming("your-name", "warn");
      or 
    LogTimes.endTiming("your-name", "warn", "your-description");
    `
  **Logging level 'error'**
    <br>`LogTimes.startTiming("your-name"); 
    LogTimes.endTiming("your-name", "error");
      or
    LogTimes.endTiming("your-name", "error", "your-description");
    `
	
# General Info

## GIT Strategy
* Open command line and move to your workspace.
* Download project using your username: 
<br>`> git clone https://github.com/kmponis-nhs/performance-indicator.git`
* Go to develop branch
<br>`> git checkout develop`
* Create a slave branch - using the story number (ex. sml-9)
<br>`> git branch <newBranchName>`
* Select slave branch 
<br>`> git checkout <newBranchName>`
* Add slave branch to repository 
<br>`> git push --set-upstream origin <newBranchName>`
* When story is finished push and request a merge
* Pull changes from develop
<br>`> git checkout <newBranchName>`
<br>`> git fetch origin`
<br>`> git merge origin/develop`
<br>`> git push`