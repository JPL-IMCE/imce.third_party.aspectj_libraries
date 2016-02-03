# JPL MBEE Common Scala Libraries Dependencies

This project aggregates several Scala libraries that are common dependencies
for multiple JPL MBEE components.

## Build procedure (local, Jenkins CI)

```
% sbt -Dsbt.global.staging=sbt.staging -DJPL_MBEE_LOCAL_REPOSITORY=<directory path for an existing local Maven repository> publish
```

This results in 4 sets of folders where:

- The 'lib.srcs' folder contains the sources for the jar files in 'lib'

- The 'lib.javadoc' folder contains the javadoc for the jar files in 'lib'

The 4 sets of folders are:

1. The Scala libraries (runtime, compiler, reflection)

    For details, see the ```scalaLibs``` sub-project in ```build.sbt``` 

    ```
    scalaLibs/target/pack/lib
    scalaLibs/target/pack/lib.srcs
    scalaLibs/target/pack/lib.javadoc
    ```

2. Additional Scala libraries

    For details, see the ```otherLibs``` sub-project in ```build.sbt``` 
    
    ```
    otherLibs/target/pack/lib
    otherLibs/target/pack/lib.srcs
    otherLibs/target/pack/lib.javadoc
    ```
    
3. OWL API libraries

    For details, see the ```owlapiLibs``` sub-project in ```build.sbt``` 
    
    ```
    owlapiLibs/target/pack/lib
    owlapiLibs/target/pack/lib.srcs
    owlapiLibs/target/pack/lib.javadoc
    ```

4. Scala Graph libraries

    For details, see the ```graphLibs``` sub-project in ```build.sbt``` 
    
    ```
    graphLibs/target/pack/lib
    graphLibs/target/pack/lib.srcs
    graphLibs/target/pack/lib.javadoc
    ```
