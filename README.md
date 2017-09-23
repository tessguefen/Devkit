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
### Other Examples
```xml
<mvt:item name="dev_util" param="Date('D M j, Y G:i:s a', s.time_t, l.settings:my_date)" />
Test Date: &mvt:my_date;
```


## Variant Array Output example.
```xml
<mvt:item name="dev_util" param="Variant_Array( l.settings:product_id, l.settings:output )" />
<mvt:eval expr="glosub(miva_array_serialize(l.settings:output ), ',', '<br />')" />
```
Output!:
```
[1]:attributes[1]:attmpat_id=21
[1]:attributes[1]:attr:attemp_id=8
[1]:attributes[1]:attr:code=flavor
[1]:attributes[1]:attr:cost=0
[1]:attributes[1]:attr:default_id=0
[1]:attributes[1]:attr:disporder=25
[1]:attributes[1]:attr:id=21
[1]:attributes[1]:attr:inventory=1
[1]:attributes[1]:attr:price=0
[1]:attributes[1]:attr:prompt=Flavor
[1]:attributes[1]:attr:required=1
[1]:attributes[1]:attr:type=radio
[1]:attributes[1]:attr:weight=0
[1]:attributes[1]:attr_id=98
[1]:attributes[1]:option:attemp_id=8
[1]:attributes[1]:option:attmpat_id=21
[1]:attributes[1]:option:code=cl
[1]:attributes[1]:option:cost=0
[1]:attributes[1]:option:disporder=21
[1]:attributes[1]:option:id=21
[1]:attributes[1]:option:price=0
[1]:attributes[1]:option:prompt=Cerise+Limon
[1]:attributes[1]:option:weight=0
[1]:attributes[1]:option_id=21
[1]:attributes[1]:template:code=LaCroix
[1]:attributes[1]:template:id=8
[1]:attributes[1]:template:prompt=La+Croix
[1]:attributes[1]:template:refcount=1
[1]:attributes[2]:attmpat_id=22
[1]:attributes[2]:attr:attemp_id=8
[1]:attributes[2]:attr:code=pkg
[1]:attributes[2]:attr:cost=0
[1]:attributes[2]:attr:default_id=0
[1]:attributes[2]:attr:disporder=26
[1]:attributes[2]:attr:id=22
[1]:attributes[2]:attr:inventory=1
[1]:attributes[2]:attr:price=0
[1]:attributes[2]:attr:prompt=Package
[1]:attributes[2]:attr:required=1
[1]:attributes[2]:attr:type=radio
[1]:attributes[2]:attr:weight=0
[1]:attributes[2]:attr_id=98
[1]:attributes[2]:option:attemp_id=8
[1]:attributes[2]:option:attmpat_id=22
[1]:attributes[2]:option:code=6pk
[1]:attributes[2]:option:cost=0
[1]:attributes[2]:option:disporder=24
[1]:attributes[2]:option:id=24
[1]:attributes[2]:option:price=0
[1]:attributes[2]:option:prompt=6+Pack
[1]:attributes[2]:option:weight=0
[1]:attributes[2]:option_id=24
[1]:attributes[2]:template:code=LaCroix
[1]:attributes[2]:template:id=8
[1]:attributes[2]:template:prompt=La+Croix
[1]:attributes[2]:template:refcount=1
[1]:attributes[3]:attmpat_id=23
[1]:attributes[3]:attr:attemp_id=8
[1]:attributes[3]:attr:code=free_try
[1]:attributes[3]:attr:cost=0
[1]:attributes[3]:attr:default_id=0
[1]:attributes[3]:attr:disporder=27
[1]:attributes[3]:attr:id=23
[1]:attributes[3]:attr:inventory=1
[1]:attributes[3]:attr:price=0
[1]:attributes[3]:attr:prompt=Free+Random+La+Croix%3F
[1]:attributes[3]:attr:required=0
[1]:attributes[3]:attr:type=checkbox
[1]:attributes[3]:attr:weight=0
[1]:attributes[3]:attr_id=98
[1]:attributes[3]:option_id=1
[1]:attributes[3]:template:code=LaCroix
[1]:attributes[3]:template:id=8
[1]:attributes[3]:template:prompt=La+Croix
[1]:attributes[3]:template:refcount=1
[1]:dimensions=3
[1]:overall_inventory:active=1
[1]:overall_inventory:agrpcount=0
[1]:overall_inventory:cancat_id=0
[1]:overall_inventory:catcount=2
[1]:overall_inventory:code=lacroix_yum
[1]:overall_inventory:cost=0
[1]:overall_inventory:disp_order=293
[1]:overall_inventory:dt_created=1502516550
[1]:overall_inventory:dt_updated=1503030585
[1]:overall_inventory:id=290
[1]:overall_inventory:inv_active=1
[1]:overall_inventory:inv_available=0
[1]:overall_inventory:inv_instock=0
[1]:overall_inventory:inv_level=out
[1]:overall_inventory:inv_long=Sorry%2C+we+are+currently+sold+out+of+%27La+Croix%27.+Please+check+back+later.
[1]:overall_inventory:inv_low_level=0
[1]:overall_inventory:inv_low_track=0
[1]:overall_inventory:inv_out_level=0
[1]:overall_inventory:inv_out_track=1
[1]:overall_inventory:inv_short=Sold+Out
[1]:overall_inventory:name=La+Croix
[1]:overall_inventory:page_id=0
[1]:overall_inventory:pgrpcount=0
[1]:overall_inventory:price=99
[1]:overall_inventory:taxable=1
[1]:overall_inventory:weight=0
[1]:part_count=2
[1]:parts[1]:active=0
[1]:parts[1]:agrpcount=0
[1]:parts[1]:cancat_id=0
[1]:parts[1]:catcount=0
[1]:parts[1]:code=Master_Product_s_blue
[1]:parts[1]:cost=0
[1]:parts[1]:disp_order=280
[1]:parts[1]:dt_created=1502516104
[1]:parts[1]:dt_updated=1502653973
[1]:parts[1]:id=277
[1]:parts[1]:inv_active=1
[1]:parts[1]:inv_available=0
[1]:parts[1]:inv_instock=0
[1]:parts[1]:inv_level=out
[1]:parts[1]:inv_long=Sorry%2C+we+are+currently+sold+out+of+%27Master+Product+size%3As+color%3Ablue%27.+Please+check+back+later.
[1]:parts[1]:inv_low_level=0
[1]:parts[1]:inv_low_track=0
[1]:parts[1]:inv_out_level=0
[1]:parts[1]:inv_out_track=1
[1]:parts[1]:inv_short=Sold+Out
[1]:parts[1]:name=Master+Product+size%3As+color%3Ablue
[1]:parts[1]:page_id=0
[1]:parts[1]:pgrpcount=0
[1]:parts[1]:price=0
[1]:parts[1]:quantity=1
[1]:parts[1]:taxable=1
[1]:parts[1]:weight=0
[1]:parts[2]:active=0
[1]:parts[2]:agrpcount=0
[1]:parts[2]:cancat_id=0
[1]:parts[2]:catcount=0
[1]:parts[2]:code=lacroix_yum_cl_6pk_free_tryY
[1]:parts[2]:cost=0
[1]:parts[2]:disp_order=296
[1]:parts[2]:dt_created=1502516596
[1]:parts[2]:dt_updated=1502516596
[1]:parts[2]:id=293
[1]:parts[2]:inv_active=1
[1]:parts[2]:inv_available=0
[1]:parts[2]:inv_instock=0
[1]:parts[2]:inv_level=out
[1]:parts[2]:inv_long=Sorry%2C+we+are+currently+sold+out+of+%27La+Croix+flavor%3Acl+pkg%3A6pk+free_try%3AChecked%27.+Please+check+back+later.
[1]:parts[2]:inv_low_level=0
[1]:parts[2]:inv_low_track=0
[1]:parts[2]:inv_out_level=0
[1]:parts[2]:inv_out_track=1
[1]:parts[2]:inv_short=Sold+Out
[1]:parts[2]:name=La+Croix+flavor%3Acl+pkg%3A6pk+free_try%3AChecked
[1]:parts[2]:page_id=0
[1]:parts[2]:pgrpcount=0
[1]:parts[2]:price=0
[1]:parts[2]:quantity=1
[1]:parts[2]:taxable=1
[1]:parts[2]:weight=0
[1]:product_id=290
[1]:variant_id=334
```
