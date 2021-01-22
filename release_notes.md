# Release Notes

This page contains the important feature changes.

| version | new stuff |
| -- | -- | 
| 3.5.0 | <ul><li>Upgrade Bootstrap from 4.5.2 to 4.6.0</li><li>Replace popper.js by @popperjs/core</li></ul> | 
| 3.4.2 | Upgrade Bootstrap from 4.5.1 to 4.5.2 | 
| 3.4.1 | Upgrade Bootstrap from 4.5.0 to 4.5.1 | 
| 3.4.0 | Upgrade Bootstrap from 4.4.1 to 4.5.0 | 
| 3.3.3 | Increase javascript and css resource compression | 
| 3.3.2 | Fixed issue #263 (TreeBox does not work after update dependency) |
| 3.3.1 | <ul><li>Fixed issue #259 (NPE on number component)</li><li>Bump npm and node to latest version</li></ul> | 
| 3.3.0 | Upgrade Bootstrap from 4.3.1 to 4.4.1 | 
| 3.2.0 | Switch to Jakarta EE 8 | 
| 3.1.3 | <ul><li>Textarea: Fixed misleading character count</li><li>Number: Fixed initializing Component with 0 when clicking buttons first time</li><li>Radiobox: Fixed alignment</li></ul> | 
| 3.1.2 | <ul><li>Fixed critical ajax bug when using JSF2.3</li><li>Fixed calendar when using ajax function</li></ul> |
| 3.1.1 | <ul><li> Upgrade jQuery from 3.3.1 to 3.4.1</li><li>Upgrade inputmask from 3.3.11 to 4.0.8</li><li>Upgrade popper.js from 1.14.7 to 1.15.0</li><li>Upgrade typescript from 3.3.3333 to 3.4.5</li><li>Activate JDK 12 build</li></ul> |
| 3.1.0 | Upgrade Bootstrap from 4.2.1 to 4.3.1 |
| 3.0.7 | <ul><li>Upgrade Bootstrap to 4.2.1</li><li>Fixes showcase tags distinct bug</li><li>Replace custom checkbox switch by new Bootstrap feature</li><li>Upgrade trivial components to 0.1.20</li><li>Upgrade Calendar component Tempus Dominus to 5.1.2</li></ul> | 
| 3.0.6 | <ul><li>Upgrade Calendar component Tempus Dominus to 5.1.1</li><li>Fixed input component height</li><li>Fixed input component width when hideLable property is set</li><li>Automatically close tooltip on blur input component</li><li>Add web.xml parameter org.butterfaces.tooltip.position.label to add tooltip to label instead of whole component</li></ul>| 
| 3.0.5 | Upgrade Bootstrap from 4.1.2 to 4.1.3| 
| 3.0.4 | Upgrade Bootstrap from 4.1.1 to 4.1.2 |
| 3.0.3 | Upgrade Calendar component Tempus Dominus to 5.0.1 |
| 3.0.2 | Upgrade Bootstrap to 4.1.1 |
| 3.0.1 | Fixed client side table filtering |
| 3.0.0 | JEE 8 release of 3.0.0-JEE7. JEE8 is required. See 3.0.0-JEE7 for release notes. |
| 3.0.0-JEE7 | <ul><li>Upgrade Bootstrap from 3.3.7 to 4.0.0</li><li>Upgrade calendar component javascript to a new Bootstrap 4 version with more locale support</li><li>Add switch attribute to checkbox component to enable a toggle behaviour</li><li>Introduce showdown.js 1.8.6 to support more markdown features</li><li>Upgrade javascript library trivial components to 0.1.16</li><li>Upgrade javascript library jQuery to 3.2.1</li><li>Introduce javascript library popper.js 1.12.9</li><li>Upgrade miscellaneous dev javascript library to latest versions (like typescript)</li><li>Removed bower from build process</li><li>All de.larmic.butterfaces packages has been renamed to org.butterfaces</li><li>Maven groupId has been renamed from de.larmic.butterfaces to org.butterfaces</li></ul> |
| 2.1.25 | Fixed issue #127 (fixed position of validation message on calendar component) |
| 2.1.24 | Fixed issue #120 (fixed validation on required fields with empty space) |
| 2.1.23 | Fixed issue #123 (markdown javascript fix) |
| 2.1.22 | Fixed issue #121 (cross site scripting) |
| 2.1.21 | Fixed issue when using semicolon in command link id |
| 2.1.20 | Fixed issue when using calendar component without language. In this case browser language will be used. |
| 2.1.19 | <ul><li>Upgrade showcase wildfly swarm to latest release</li><li>Prepare docker image for showcase</li><li>#97 Fixed issue using ' in tags component</li></ul> |
| 2.1.18 | Add web.xml parameter to toggle "showClearButton" in b:treeBox |
| 2.1.17 | Some dependency maintenance like upgrade wildfly swarm |
| 2.1.15 | Bugfixing building javascript bundles for inputmask jQuery plugin |
| 2.1.14 | Bugfixing issue when using tags component without white space as confirm key |
| 2.1.13 | Bugfixing ajax problem with TreeBox component. |
| 2.1.12 | <ul><li>Update trivial components to latest version</li><li>Update dateTimePicker to latest version</li><li>Technical updates like nodejs and bower</li></ul> |
| 2.1.11 | <ul><li>Fixed z-index of TreeBox component when using modal panels.</li><li>Improved toString() usage in TreeBox component</li></ul> |
| 2.1.10 | <ul><li>Upgrade JQuery from 2.1.4 to 2.2.4</li><li>Upgrade Bootstrap from 3.3.6 to 3.3.7</li></ul>  |
| 2.1.9 | Fixed ignoring mustache keys in TreeBox component. |
| 2.1.8 | Better PrimeFaces integration. No additional configuration is needed. It works out-of-the-box. |
| 2.1.7 | Add multiline placeholder support for textarea and markdown components |
| 2.1.6 | Fixed using autoComplete without using f:ajax |
| 2.1.5 | Clicking on label will set focus to input components (except trivial components) |
| 2.1.4 | <ul><li>New faster table component</li><li>tree component supports style and styleClass attribute</li><li>Repeat component receives status attribute</li><li>maskedText component supports more functions of inputMask-javascript plugin</li></ul> |
| 2.1.3 | Accelerate ajax rendering of table component up to factor 2.5 |
| 2.1.2 | Fixed localization bug in character counter of testarea component |
| 2.1.1 | web.xml parameter org.butterfaces.maxLengthText allows to use custom text for textarea and markdown counter |
| 2.1.1 | Fix a problem with b:repeat and MyFaces 2.1.x |
| 2.1.0 | <ul><li>Fixed autocomplete bug when using MyFaces 2.1.x</li><li>Fixed ajax bug when using MyFaces 2.1.x</li><li>Radiobox components comes with template support</li></ul> |
| 2.0.0 | <ul><li>combobox has been removed and replaced by treebox</li><li>new web.xml parameter org.butterfaces.autoTrimInputFields activates auto trim for input fields (true by default)</li></ul>
| 2.0.0.CR1 | [radioBox](http://www.butterfaces.org/butterfaces-showcase/radiobox.jsf) relieves Mojarra |
| 1.11.1 | <ul><li>treeBox component comes with dot notation support for mustache syntax</li><li>ajaxDisableRenderRegionsOnRequest is supported by web.xml</li><li>noEntriesText is supported by web.xml</li><li>Fix bug when using readonly checkbox and form submit</li></ul> |
| 1.11.0 | [table component](http://www.butterfaces.org/butterfaces-showcase/table.jsf) relieves Mojarra and Bootstrap upgrade from 3.3.5 to 3.3.6 |
| 1.10.5 | Second CR of [treeBox component](http://www.butterfaces.org/butterfaces-showcase/treebox.jsf)|
| 1.10.4 | <ul><li>First CR of treeBox component</li><li> checkbox component relieves Mojarra</li></ul>|
| 1.9.14 | [textarea component ](http://www.butterfaces.org/butterfaces-showcase/textarea.jsf) relieves Mojarra|
| 1.9.13 | [new repeat component ](http://www.butterfaces.org/butterfaces-showcase/repeat.jsf)|
| 1.9.0 | <ul>	<li>All text components are MyFaces compatible</li><ul><li>Calendar</li><li>Tags</li><li>Text</li><li>MaskedText</li><li>Secret</li><li>Number</li></ul><li>Tags component switched to https://trivial-components.github.io/trivial-components/. It comes with a new design.</li><li>Tree component switched to https://trivial-components.github.io/trivial-components/. It comes with a new design.</li><li>ButterFaces code has been moved to GitHub</li>|
| 1.8.4 |Table columns ordering support|
| 1.7.13 | [new tooltip component](http://www.butterfaces.org/butterfaces-showcase/tooltip.jsf) |



