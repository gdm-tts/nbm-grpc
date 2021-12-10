# nbm-grpc

Simple Maven NetBeans Module to test error when gRPC depencendies are added.

To reproduce, clone the reposiotry, open the project in NetBeans 12.6 and clean&build.

Should also work from the command line:
```
mvn clean install
```

Output:
> ```Failed to execute goal org.apache.netbeans.utilities:nbm-maven-plugin:4.6:manifest (default-manifest) on project standalone-grpc-module: Uncategorized problems with NetBeans dependency verification (maybe MNBMODULE-102 or wrong maven dependency metadata). Supposedly external classes are used in the project's binaries but the classes are not found on classpath. Class usages: [io.perfmark.Tag, android.annotation.SuppressLint, com.google.gson.stream.JsonToken, io.perfmark.Link, io.perfmark.PerfMark, com.google.gson.stream.JsonReader, org.codehaus.mojo.animal_sniffer.IgnoreJRERequirement]```
