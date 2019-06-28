# Assumptions of automated tests

* Test should be easy to maintenance.

* Common aprroach to / common nomenclature for:
  * How will we tests
  * A comprehensive test scenario 
  * Style of testing writing (given, when, then approach etc.)
  * The whole naming of test (elements, name of methods etc.)

* Asserts
  * Each assert has separate comment

* Keep test logic outside the product code. Create separate test framework for that.  

* Don't adjustment product to tests.

* Creating data for test should be: 
  * injecting to database 
  * created by service layer

* Prepare environment and cleaning must be outside the test. 
