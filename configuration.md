# Configuration

This part contains the options to customize ButterFaces by editing `web.xml`.

* [Using of jQuery](#JQuery)
* [Using of Bootstrap](#Bootstrap)
* [Ajax configuration](#Ajax)
* [Auto trim input fields](#autoTrim)
* [Max length text](#maxLength)
* [Tree configuration](#Tree)
* [PrimeFaces integration](#PrimeFacesIntegration)
* [Resourcehandling](#Resourcehandling)

*HINT* with version 2.0.0 web.xml parameters has been renamed from de.larmic.butterfaces.x to org.butterfaces.x

<a name="JQuery"></a>
## Using of jQuery

As default ButterFaces comes with an actual version of jQuery 3.x. To disable ButterFaces jQuery version because of using your own version you have to change following parameter

```xml
<context-param>
	<param-name>org.butterfaces.provideJQuery</param-name>
	<param-value>false</param-value>
</context-param>
```

<a name="Bootstrap"></a>
## Using of Bootstrap

As default ButterFaces comes with an actual version of Bootstrap 3.x. To disable ButterFaces Boostrap version because of using your own version you have to change following parameter

```xml
<context-param>
	<param-name>org.butterfaces.provideBootstrap</param-name>
	<param-value>false</param-value>
</context-param>
```

<a name="Ajax"></a>
## Ajax configuration 
> (since 1.11.1)

*b:commandLink* components comes with **ajaxDisableRenderRegionsOnRequest** to crossfade render regions while ajax request is running. To configure this for global usage add following parameter

```xml
<context-param>
	<param-name>org.butterfaces.ajaxDisableRenderRegionsOnRequest</param-name>
	<param-value>false</param-value>
</context-param>
```
This can be useful if you are using *b:waitingPanel* to disable *b:commandLink* support and to prevent multiple crossfade windows.

<a name="autoTrim"></a>
## Auto trim input fields
> (since 2.0.0)

By default all input fields will be trimed after submit. 

```xml
<context-param>
	<param-name>org.butterfaces.autoTrimInputFields</param-name>
	<param-value>true</param-value>
</context-param>
```

<a name="maxLength"></a>
## Max length text for textArea and markdown
> (since 2.1.2)

When using maxlength parameter counting text will be *{0} of {1} characters*.

```xml
<context-param>
	<param-name>org.butterfaces.maxLengthText</param-name>
	<param-value>{0} of {1} characters</param-value>
</context-param>
```

<a name="Tree"></a>
## Tree configuration 
> (since 1.11.1)

b:tree and b:treeBox are trivial components and can be configured by components attribute or by changeing following parameters

```xml
<context-param>
	<param-name>org.butterfaces.noEntriesText</param-name>
	<param-value>No matching entries...</param-value>
</context-param>
<context-param>
	<param-name>org.butterfaces.spinnerText</param-name>
	<param-value>Fetching data...</param-value>
</context-param>
```

<a name="PrimeFacesIntegration"></a>
## PrimeFaces integration
> (since 2.1.8)

As well as ButterFaces PrimeFaces comes with jQuery. By default PrimeFaces JQuery will be removed from resources. You can change this behaviour by changeing following parameter

```xml
<context-param>
	<param-name>org.butterfaces.integration.primefaces.disableJQuery</param-name>
	<param-value>true</param-value>
</context-param>
```

<a name="Resourcehandling"></a>
## Resourcehandling

Each components comes up with it's own javascript and css resources. If you want to use ButterFaces resources (i.e. Bootstrap or jQuery) without any ButterFaces component use [b:activateLibraries](http://www.butterfaces.org/butterfaces-showcase/activateLibraries.jsf) to load all resources to html

```xml
<!DOCTYPE html>
<html lang="en"
      xmlns:h="http://xmlns.jcp.org/jsf/html"
      xmlns:ui="http://xmlns.jcp.org/jsf/facelets"
      xmlns:b="http://butterfaces.org/components"
      xmlns:f="http://xmlns.jcp.org/jsf/core">
      ...
    <b:activateLibraries />
</html>```
This tags add javascript and css resources for all existing components. In addition to that you may activate compression by web.xml
```xml
<context-param>
    <param-name>org.butterfaces.useCompressedResources</param-name>
    <param-value>true</param-value>
</context-param>```

*HINT* This only works if you are using 
```xml
<context-param>
    <param-name>javax.faces.PROJECT_STAGE</param-name>
    <param-value>Production</param-value>
</context-param>
```
When using `Development`resource will always provided as non minified and compressed. Likewise sourcemaps will be supplied to enable javascript debugging.

