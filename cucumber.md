### Cucumber Framework
	Cucumber is a software testing framework that supports behavior-driven development (BDD). It is used for 
	writing tests in a natural language format that is easily readable by both technical and non-technical 
	stakeholders. The tests are written in a Gherkin format, which specifies the behavior being tested in a
	series of steps.
	
	 It's primarily used to develop acceptance tests for web apps
	 
### Sample script
	Feature: Login
	  As a user,
	  I want to be able to log in to the system
	  So that I can access my account information

	Scenario: Successful Login
	  Given the user is on the login page
	  When the user enters their username and password
	  And clicks the "Login" button
	  Then the user should be taken to the home page
	  And a message should be displayed that says "Welcome, [username]"

	Scenario: Unsuccessful Login
	  Given the user is on the login page
	  When the user enters an incorrect username and password
	  And clicks the "Login" button
	  Then an error message should be displayed that says "Incorrect username or password."
