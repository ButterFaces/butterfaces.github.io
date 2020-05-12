# Getting started

## Install ButterFaces as maven dependency

ButterFaces is accessible by [maven central repository](http://search.maven.org/#search/ga\|1\|butterfaces). Add following dependency to use components for each JSF implementation \(i.e. MyFaces\).

```xml
<dependency>
    <groupId>org.butterfaces</groupId>
    <artifactId>components</artifactId>
    <version>3.4.0</version>
</dependency>
```

Pre 3.0.0 versions of ButterFaces comes with JQuery 2.latest and Bootstrap 3.latest

```xml
<dependency>
    <groupId>de.larmic.butterfaces</groupId>
    <artifactId>components-mojarra</artifactId>
    <version>2.1.25</version>
</dependency>
```

## Install ButterFaces by yourself

You can clone git repository and install maven plugin by yourself using console

```
git@github.com:ButterFaces/ButterFaces.git
maven install
```

## Using ButterFaces

Add `http://butterfaces.org/components` to your `<html .../>` and use `<!DOCTYPE html>` to activate html 5 features.

```xml
<!DOCTYPE html>
<html lang="en"
      xmlns:h="http://xmlns.jcp.org/jsf/html"
      xmlns:ui="http://xmlns.jcp.org/jsf/facelets"
      xmlns:b="http://butterfaces.org/components"
      xmlns:f="http://xmlns.jcp.org/jsf/core">
      ...
    <b:text id="test" ... />
</html>
```

That's all!

