# BootsFaces integration

As well as ButterFaces [BootsFaces](http://www.bootsfaces.net/) comes with jQuery and Bootstrap. This does not work out of the box.

## Problem
ButterFaces deliveres css and javascript as first part of html head to allow custom class handling. BootsFaces deliveres its own jQuery after ButterFaces, so ButterFaces jQuery plugins does not work anymore.

## Solution
Disable jQuery in BootsFaces and most things will work
```xml
<context-param>
    <param-name>net.bootsfaces.get_jquery_from_cdn</param-name>
    <param-value>true</param-value>
</context-param>
```

## Known problems
BootsFaces and ButterFaces override some Bootstrap style sheet. Sometimes they come in the transverse, i.e. placeholder position in ButterFaces. We are working on that.

## Code example
Take a look at https://github.com/ButterFaces/bootsfaces-integration