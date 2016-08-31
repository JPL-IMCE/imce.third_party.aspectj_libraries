# IMCE Third-Party AspectJ Libraries

[![Build Status](https://travis-ci.org/JPL-IMCE/imce.third_party.aspectj_scala_libraries.svg?branch=master)](https://travis-ci.org/JPL-IMCE/imce.third_party.aspectj_scala_libraries)
[ ![Download](https://api.bintray.com/packages/jpl-imce/gov.nasa.jpl.imce/imce.third_party.aspectj_scala_libraries/images/download.svg) ](https://bintray.com/jpl-imce/gov.nasa.jpl.imce/imce.third_party.aspectj_scala_libraries/_latestVersion)
 
This project builds an aggregate of the AspectJ libraries published by the following organization:

- [org.aspectj](http://www.eclipse.org/aspectj/) A seamless aspect-oriented extension to the Java programming language.

## Usage

```
    resolvers += Resolver.bintrayRepo("jpl-imce", "gov.nasa.jpl.imce"),

    libraryDependencies += 
      "gov.nasa.jpl.imce" %% "imce.third_party.aspectj_scala_libraries" % "<version>"
        artifacts
        Artifact("imce.third_party.aspectj_scala_libraries", "zip", "zip", Some("resource"), Seq(), None, Map())
```