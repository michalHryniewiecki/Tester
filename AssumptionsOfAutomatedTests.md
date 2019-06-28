# Assumptions of automated tests

1. Test should be easy to maintenance.

2. Common aprroach to / common nomenclature for:
- How will we tests
- A comprehensive test scenario 
- Style of testing writing (given, when, then approach etc.)
- The whole naming of test (elements, name of methods etc.)

3. Asserts
- Each assert has separate comment
...

4. Keep test logic outside the product code. Create separate test framework for that.  

5. Don't adjustment product to tests.

6. Creating data for test should be: 
- injecting to database 
- created by service layer

7. Prepare environment and cleaning must be outside the test. 
