# JAVACoding
It may helpful for Writing good Java code,Java Coding Standard and Improve the Java Code Quality


1.Java Coding Standard (Beginner/Intermediate Level): fallow below link

https://oss-generic.github.io/process/codingStandards/CodingStandard-Java.html

2.Writing good Java code:

https://developer.ibm.com/tutorials/j-perry-writing-good-java-code/

3.Java Code Conventions by Oracle Corp

Link : https://www.oracle.com/technetwork/java/codeconventions-150003.pdf 

4.Blog for JAVA

https://blogs.oracle.com/java/java

5.Logging in Java

https://stackify.com/java-logging-best-practices/

6.Use StringBuilder to concatenate Strings programmatically

7.Use primitives where possible

8.Try to avoid BigInteger and BigDecimal

9. Check the current log level first
This recommendation should be obvious, but unfortunately, you can find lots of code that ignores it. Before you create a debug message, you should always check the current log level first. Otherwise, you might create a String with your log message that will be ignored afterward.

Here are 2 examples of how you should NOT do it.

// don’t do this
log.debug(“User [” + userName + “] called method X with [” + i + “]”);
// or this
log.debug(String.format(“User [%s] called method X with [%d]”, userName, i));

In both cases, you will perform all required steps to create the log message without knowing if your logging framework will use the log message. It’s better to check the current log level first before you create the debug message.

// do this
if (log.isDebugEnabled()) {
log.debug(“User [” + userName + “] called method X with [” + i + “]”);
}

#Java performance tuning tips
https://www.javaperformancetuning.com/tips/rawtips.shtml








