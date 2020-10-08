# Developer Testing with JUnit 

This exercise introduces how testing is done by developers and using the JUnit test framework for unit testing.

The implementation of a _RingBuffer_ (from the draft version of Introduction to Programming in Java: An Interdisciplinary Approach, R. Sedgewick and K. Wayne, Addison-Wesley, 2008) is the class under  test.

## RingBufferTest _(2 points)_

The task is to write 4 unit tests for the class RingBuffer. The goal is not to write many unit tests but to write useful unit tests that correctly use the [JUnit framework](https://junit.org/junit5/docs/current/user-guide/#writing-tests).

### Instructions

- Name the test class containing the tests `at.fhhagenberg.sqe.RingBufferTest` and put it into the folder `src/test/java`.
- The test cases (test methods in the class `RingBufferTest`) should test different aspects/features of the implementation. Try to find positive test cases that show the typical behavior of a ring buffer.
- Name each test method with the prefix _test<MethodName>_ (e.g., `testFooBar()`).
- If you find a bug in the implementation of RingBuffer, demonstrate it by a failing (red) test.

> Run your tests with `mvn test` in a new shell. The result should be similar to:

```
-------------------------------------------------------
 T E S T S
-------------------------------------------------------
Running at.fhhagenberg.sqe.RingBufferTest
Tests run: 3, Failures: 0, Errors: 0, Skipped: 0, Time elapsed: 0.016 sec

Results :
Tests run: 3, Failures: 0, Errors: 0, Skipped: 0

[INFO] ------------------------------------------------------------------------
[INFO] BUILD SUCCESS
[INFO] ------------------------------------------------------------------------
[INFO] Total time:  6.837 s
[INFO] Finished at: 2020-10-02T09:17:44+02:00
[INFO] ------------------------------------------------------------------------
```

### Submission

When you're done...

- [x] push your changes to your upstream repository on GitHub.
- [x] on GitHub, [create a release][GitHub creating releases] with version `v0.1`.
- [x] upload the [link to your release][GitHub linking to releases] on the e-learning platform until the specified date and time before the next lecture.
- [x] Only complete submissions adhering to all of the above requirements are considered. Late submissions, submissions via email or submissions failing to meet the specified requirements will not be accepted.

## EmptyRingBufferTest _(2 points)_

### Instructions

Write another test class _EmptyRingBufferTest_ containing tests for an empty RingBuffer. Put these tests in a separate test class because they use a different test fixture (setup). 

- Name the test class `at.fhhagenberg.sqe.EmptyRingBufferTest`.
- Provide at least 1 test case. This test should provoke an exception. Make sure the expected exception is actually thrown and check the exception type, message, etc. 

### Submission

When you're done...

- [x] push your changes to your upstream repository on GitHub.
- [x] on GitHub, [create a release][GitHub creating releases] with version `v0.2`.
- [x] upload the [link to your release][GitHub linking to releases] on the e-learning platform until the specified date and time before the next lecture.
- [x] Only complete submissions adhering to all of the above requirements are considered. Late submissions, submissions via email or submissions failing to meet the specified requirements will not be accepted.


[GitHub creating releases]: https://help.github.com/articles/creating-releases/
[GitHub linking to releases]: https://help.github.com/articles/linking-to-releases/
