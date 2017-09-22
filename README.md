# developer_utilities

All the things!

Steven:

```xml
<mvt:assign name="l.params:code" value="'my-product-code'" />
<mvt:assign name="l.params:include" value="'attributes,inventory,runtime_price'" />
<mvt:assign name="l.params:image_types" value="'main:500x500,alt_1:500x500'" />
<mvt:assign name="l.params:custom_fields" value="'brand,price_range'" />
<mvt:assign name="l.params:cached" value="1" />

<mvt:do file="g.Module_DevKit" name="l.result" value="Load_Product(l.params, l.product)" />



<mvt:assign name="l.params:codes" value="'code-123,code-456,code-789'" />

<mvt:do file="g.Module_DevKit" name="l.result" value="Load_Products(l.params, l.products)" />
```
