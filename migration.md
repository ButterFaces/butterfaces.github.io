# Migration

This page shows migration instructions if some ButterFaces version require it.

| from version | to version | what to do |
| -- | -- | -- |
| >= 2.1.2 | 3.0.0 | <ul><li>See 3.0.0-JEE7 migration stuff</li><li>JEE8 is required</li></ul> |
| >= 2.1.2 | 3.0.0-JEE7 | <ul><li>Bootstrap is updated from 3.3.7 to 4.0.0. ButterFaces 3 does not support Bootstrap 3.x anymore. Follow [Bootstrap migration guide](https://getbootstrap.com/docs/4.0/migration/) to upgrade your custom components</li><li>Calendar tag attribute language has been renamed to locale</li><li>jQuery is updated from latest 2.x to 3.2.1. ButterFaces 3 is compatible with jQuery 2 but you have to add your own version of jQuery described [here](https://butterfaces.gitbooks.io/butterfaces/content/configuration.html#JQuery)</li><li>All de.larmic.butterfaces packages has been renamed to org.butterfaces.</li><li>Maven dependency de.larmic.butterfaces has been renamed to org.butterfaces</li></ul> |
| 2.1.1 | 2.1.2 | Use web.xml parameter <i>org.butterfaces.maxLengthText</i> to localize text area max length text |
| 2.0.0.CR1 | 2.0.0 | <ul><li>combobox components has been removed (use treebox instead)</li><li>components namespace has been changed from http://butterfaces.larmic.de/components to  http://butterfaces.org/components</li><li>web.xml parameters has been renamed from de.larmic.butterfaces.x to org.butterfaces.x</li><li>web.xml parameter ajaxDisableRenderRegionsOnRequest has been renamed to org.butterfaces.ajaxDisableRenderRegionsOnRequest</li></ul>
| 1.9.14 | 1.9.15 | <ul><li>TreeBox hideRootNode has removed.</li><li>Use List<Node> instead of Node as treeBox value if you want to hide root node</li></ul> |
| 1.9.6 | 1.9.8 | <ul><li>Javascript migrated to Typescript</li><li>	butter.disableElements has replaced by new ButterFaces.Overlay()</li></ul> |
| 1.8.17 | 1.9.0 | <ul>	<li>ButterFaces code has been moved to GitHub</li><li>Tree model Node.java comes with a description attribute. You may have to extend your custom model</li><li>web.xml parameters de.larmic.butterfaces.glyphicon.collapsing and de.larmic.butterfaces.glyphicon.expansion is no longer supported</li> |
| 1.8.7.1 | 1.8.8 |TreeNodeSelectionListener has a new Methode <br/>```boolean isValueSelected(final Node data);``` |
| 1.8.5 | 1.8.6 |<ul><li>TableSortModel has been renamed to TableRowSortingModel</li><li>TableColumnDisplayModel has been renamed to TableColumnVisibilityModel</li><li>showColumn and hideColumn has been refactored to update(de.larmic.butterfaces.model.table.TableColumnVisibilty)</li><li>TableOrderModel has been renamed to TableColumnOrderingModel</li><li>orderColumnToPosition has been refactored to update(de.larmic.butterfaces.model.table.TableColumnOrdering)</li></ul> |
| 1.8.4 | 1.8.5 | TableSingleSelectionListener has a new Method<br/> ```boolean isValueSelected(final T data);``` |
| 1.7.21 | 1.8.2 |Combobox component is filterable at default. Attribute filterable has been removed. |
| 1.7.16 | 1.7.17 | Table models signature has been changed |
| 1.7.12 | 1.7.13 | tooltip attribute is no longer supported. If you are using tooltips you have to replace tooltip attribute by [new tooltip component](http://www.butterfaces.org/butterfaces-showcase/tooltip.jsf) as child |



