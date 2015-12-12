# QuickTestAutomation

Reduce the testing effort with test - injection. 

The overall objective is to simplyfy unit testing using Java's reflection. If a class contains only primitive types as parameters and return types, the framework should be able to test the methods using various pre-defined test cases and values. Or if a class has to be tested against generic types, define the parameters and return values in test beans.

Example:

TestAutomator testAutomator = new TestAutomator(class);

testAutomator.runAllTests();  // Runs tests on all primitive methods.

testAutomator.runTestOn(String methodName, parameters...., return type);  // Runs tests with given i/p and expected o/p.

testAutomator.runTestOn(String methodName, parameters...., return type).testTypes(..predefined Test types); // Runs tests with defined test types.
