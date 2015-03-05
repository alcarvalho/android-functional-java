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

## IntelliJ configuration on Mac OS X

The only way IntelliJ's Gradle import would not fail for me with this
[error](https://github.com/evant/gradle-retrolambda/issues/74), was by running
[this gist](https://gist.github.com/alcarvalho/26fb041de96f6cf30e91) and restarting it.
