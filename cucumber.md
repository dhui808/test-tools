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

### How Cucumber interact with applications?
	Cucumber interacts with applications by executing the steps defined in the Cucumber scripts and comparing the 
	actual behavior of the application to the expected behavior specified in the scripts.

	Each step in a Cucumber script maps to a step definition, which is a piece of code that implements the behavior 
	described by the step. The step definitions interact with the application under test by calling its APIs, 
	clicking buttons, filling in forms, and so on.

	To implement the step definitions, you will typically use a testing library such as Ruby's RSpec, Java's JUnit, 
	or JavaScript's Mocha. These libraries provide the tools and assertions that you need to verify that the 
	application behaves as expected.

	When you run a Cucumber script, Cucumber will execute each step in the script and call the corresponding step 
	definition. If the step definition successfully executes and the actual behavior of the application matches the 
	expected behavior, the step is marked as passed. If the step definition fails or the actual behavior does not 
	match the expected behavior, the step is marked as failed and a failure message is generated.
	
