# developer_utilities

All the things!

## Load_Product(s)

```xml
<mvt:assign name="l.options:code" value="'my-product-code'" />
<mvt:assign name="l.options:include" value="'attributes,inventory,runtime_price'" />
<mvt:assign name="l.options:image_types" value="'main:500x500,alt_1:500x500'" />
<mvt:assign name="l.options:custom_fields" value="'brand,price_range'" />
<mvt:assign name="l.options:cached" value="1" />

<mvt:item name="developer_utils" param="Load_Product(l.options, l.product)" />



<mvt:assign name="l.options:codes" value="'code-123,code-456,code-789'" />

<mvt:item name="developer_utils" param="Load_Products(l.options, l.products)" />
```
