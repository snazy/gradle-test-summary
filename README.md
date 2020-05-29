Print a summary after each executed `Test` task that looks like this:

```
------------------------------------------------------------------------------------------------------------------------
|  Test Run :testUnit
|  Result: SUCCESS  (925 tests, 925 successes, 0 failures, 0 skipped, 0 exceptions)
|  Duration: 1m13.076s
|  maxParallelForks: 9
------------------------------------------------------------------------------------------------------------------------
```

For test runs using Gradle Enterprise Distributed Testing, the summary looks like this:

```
------------------------------------------------------------------------------------------------------------------------
|  Distributed Test Run :testUnit
|  Result: SUCCESS  (925 tests, 925 successes, 0 failures, 0 skipped, 0 exceptions)
|  Duration: 1m13.076s
|  local-forks: 9 - remote-test-agents: 20
------------------------------------------------------------------------------------------------------------------------
```

Usage:

```
plugins {
    id("org.caffinitas.gradle.testsummary") version "0.1.1"
}
```
