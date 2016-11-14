## Setup JUnit

### JUNIT_HOME
Assign the JUNIT_HOME environment variable and copy the minimum jars there.

~~~bash
$ ls $JUNIT_HOME
hamcrest-core-1.3.jar    junit-4.12.jar
~~~

### Try It Out

#### TestBasic.java

~~~java
import junit.framework.TestCase;

public class TestBasic extends TestCase {
  public void testTrue() {
    assertTrue(true);
  }
}
~~~

#### Run it

~~~bash
$ java org.junit.runner.JUnitCore TestBasic
JUnit version 4.12
.
Time: 0.004

OK (1 test)
~~~

