# Android Functional Java Sample

This is a sample project to try to include [functional java](http://www.functionaljava.org/) library on Android apps
with support for Java 8 lambdas.

It was created using a Mac OS X system, so there are somethings hard coded to it, i.e. it looks for Java home
using `/usr/libexec/java_home`.

## Config

You must set certain environment variables to make it work if you're not on Mac OS X:

- `JAVA8_HOME` as path to Java 8
- `JAVA7_HOME` as path to Java 7

Or you can set these using a `local.properties` file:

```
retrolambda.jdk=<path to Java 8>
retrolambda.oldJdk=<path to Java 7>
```

## Additional configuration on Mac OS X

To make it work on my Mac OS X, the only way Gradle would not fail with this error: evant/gradle-retrolambda#74

In that case, you can you this [gist](https://gist.github.com/alcarvalho/26fb041de96f6cf30e91) to it up.
