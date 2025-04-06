## React testing

## What is testing
Before deploy any application on to production it needs to make sure that all the module implemented in the applcation are working fine or should be validated and find errors of software production before launched.

## Type of testing 
Testing can be done with two different roles by developer and another QA
if testing are going with tester the it will be two types

### QA Testing
1. Manual ( Test each modules one by one manually )
2. Automation - Tester write some script which wil be run automatically ( With selenioum or other testing automation tools )

### Developer Testing
1. Unit Testing  - Testing individual unit or components
2. Integrated testing - Testing between two units or components
3. E-2-E testing - Test start to end testing of complete project

## Why developer write test
Because he wrote the source code and he know about the acceptance criteria of modules so he can write tesing easily. But the same thing QA will take much more time then developer. And another thing developer think like if he had write evverything the he wants to test the function at their end. If he is making changes one then another then he needs to test each and every time then it will consume the lot of time as well. that's why if he will write the test casse to test and functionality the it will run automatically and show the error if application not working as expected. 
Note- In developer testing if anything failed the it shows error with detail that from where the error is ccoming from and he can fix easily but in same QA can only tell that the functionality not working as expected he will not explain about error from where it is  comming

## 

We need to import only render and screen object from react-testing-library
expect() is the function of jest which is installed globally tha's why we don't need to import it.

## Group Test

To write different test cases like api, ui, and inputs needs to create groups by using describe('', ()=>{}) so that we can write test cases as per the basis of group. we are skip(describe.skip('', ()=>{})) and only(describe.only('', ()=>{})) keyowrd to run or skip specifific test group to save their testting time. We can make the testcase as nested as well.

## OnChange/Onclick event



