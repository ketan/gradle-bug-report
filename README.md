To reproduce —

```
$ [gradle|./gradlew] clean test --tests com.foo.BarTest
Using gradle wrapper at '/Users/ketanpadegaonkar/tmp/bar/gradlew' to run '/Users/ketanpadegaonkar/tmp/bar/build.gradle':

Parallel execution is an incubating feature.
:clean
:compileJava UP-TO-DATE
:processResources UP-TO-DATE
:classes UP-TO-DATE
:compileTestJava
:processTestResources UP-TO-DATE
:testClasses
:test
Running Gradle Test Executor 1
Running com.foo.BarTest
Tests run: 1, Failures: 0, Skipped: 0, Time elapsed: 0.051 sec
Tests run: 1, Failures: 0, Skipped: 0, Time elapsed: 0.056 sec
Running Gradle Test Executor 2
Running com.foo.BooTest
Tests run: 0, Failures: 0, Skipped: 0, Time elapsed: 0.05 sec
Tests run: 0, Failures: 0, Skipped: 0, Time elapsed: 0.055 sec
Running Gradle Test Executor 3
Running com.foo.FooTest
Tests run: 0, Failures: 0, Skipped: 0, Time elapsed: 0.046 sec
Tests run: 0, Failures: 0, Skipped: 0, Time elapsed: 0.052 sec
Total tests run: 1, Failures: 0, Skipped: 0, Time elapsed: 1.073 sec

BUILD SUCCESSFUL
```
