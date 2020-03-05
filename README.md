## Install instruction

To install plugin

`cd {path_to_your_kibana_folder}`

`./bin/kibana-plugin install file://{absolute_path_to_plugin}/filter_control_7.6.0.zip`

`cp -r built_assets/css/plugins/input_control_vis/ built_assets/css/plugins/filter_control_vis/`

`rm -r optimize/bundles/*`

run kibana with:

`./bin/kibana`

Go to visualize and find FilterControls visualization.
Works fine for Options:
* Update Kibana filters on each change : true
* Use time filter : true
* Pin filters for all applications : false
And control settings:
* Multiselect : false
* Dynamic Options : false
* Size: amount of distinct values you're expecting in this field (i.e. 200 for country field)


