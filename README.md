# developer_utilities

All the things!

## Load_Product

```xml
<h2>Component</h2>

<mvt:assign name="g.options:code" value="'apple'" />
<mvt:item name="developer_util" param="Load_Product(g.options, g.product_foo)" />
<hr>
<mvt:eval expr="glosub(miva_array_serialize(g.product_foo), ',', '<br>')" />


<h2>mvt:do</h2>
<mvt:assign name="l.options:code" value="'apple'" />
<mvt:assign name="l.options:include" value="'runtime,currency,uris,url'" />
	<mvt:assign name="g.Module_Developer_Utitlities" value="g.Module_Root $ 'modules/util/developer_util.mvc'" /><mvt:comment><!-- Find way for module path global variable to be available to page by default --></mvt:comment>
<mvt:do file="g.Module_Developer_Utitlities" name="l.product_v2" value="_Load_Product(l.options)" />
<hr>
<mvt:eval expr="glosub(miva_array_serialize(l.product_v2), ',', '<br>')" />
```
