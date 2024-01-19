# Overview
This is the project that contains two modules: `module-1` and `module-2`.  

## Project Inheritance
`module-1` and `module-2` specify parent module with the help of `<parent>` tag in `pom.xml`. With this setup, our modules can now inherit some of the properties of our parent POM.
Read more about project inheritance in the [documentation](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html#project-inheritance).
```xml
<parent>
    <groupId>com.kbulat</groupId>
    <artifactId>maven-multi-module-demo</artifactId>
    <version>1.0-SNAPSHOT</version>
</parent>
```

## Project Aggregation
`maven-multi-module-demo` artifact's POM defines modules that it aggregates with the `<modules>` tag. 
Read more about project aggregation in the [documentation](https://maven.apache.org/guides/introduction/introduction-to-the-pom.html#project-aggregation).

```xml
<modules>
    <module>module-1</module>
    <module>module-2</module>
</modules>
```
