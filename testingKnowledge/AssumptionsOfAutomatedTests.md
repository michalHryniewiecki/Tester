# Assumptions of automated tests

* Test should be easy to maintenance.

* Common aprroach to / common nomenclature for:
  * How will we tests
  * A comprehensive test scenario 
  * Style of testing writing 
    * Test should be splitted in 3 clear sections that has been declared in BDD: given, when, then
      * **given** - every actions that should be made before performing test action, but only these that isn't connected with setup environment 
        e.g. enterUserLogin.
      * **when** - perform action that should be tested.
      * **then** - every assertions and checkers (for acceptance criteria for test) which take places after test. 
  * The whole naming of test (elements, name of methods etc.)
    * Test name should describe test scenario in few words.
    * Test steps should be written in Present Simple. Example: *Verify password* instead of *Verifying password*.
    * Test method should have name, following to the name convention: "shouldBe(acceptance test criteria)When(action that is under testing)"
      e.g.**shouldBeDomainUpAndRunningAfterPerformRestart**

* Keep test logic outside the product code. Create separate test framework for that.  

* Don't adjustment product to tests.

* Creating data for test should be: 
  * injecting to database 
  * created by service layer

* Prepare environment and cleaning must be outside the test. 

* Take care about generate Test Report. Remember that report should be readable and user friendly. 
  * Take care about Test Case Title
  
* Test class & Test cases
  * Make test case simple. Try to avoid more than one functionality in test scenario. 
  * Should contain only tests method. It will increase transparency test cases. 
  * Setup and cleanup methods specific for test environment should be place in diffrent classes e.g. VerifyTestEnvironment.
  * Try to avoid comments - if something requires comments it hasn't been develop as simple as possible.
  * Try to avoid hardcoded sleeps. There could be resolved in way with checking with peroid of time e.g. loop that have hard limit set to 5min, but for 10 seconds it can ask feature for status. 
  * Use containers over inheritance. If it's possible please use and develop helpers e.g. JenkinsHelper, GitHelper, JiraHelper etc.  
  
* Asserts
  * Assert methods should always print a massage with failure reason. 
