# Citation

This is a standalone widget to display the citations of a agent at OpenEBench.

![Alt text](docs/images/screenshot.png 'Screenshot')

Live demo available at : https://inab.github.io/citations-widget-OEB/

# How to

Add the build file which you can download from build/build.js and tag it into your html. You can then call the `loadCitationChart()` function. The HTML file should look like the following example:

**Note** : The class attribute on the div should be `class="opebcitations"`

```html
<!DOCTYPE html>
<html>
	<meta charset="utf-8" />

	<body>
		<div
			data-id="test"
			data-title=""
			data-h="400"
			data-legend="true"
			data-url="bioagents:mega/web/www.megasoftware.net"
			class="opebcitations"
		></div>
		<script src="./build/build.js"></script>
		<script>
			loadCitationChart();
		</script>
	</body>
</html>
```

### Attributes that can be set on the _<div\>_ tag

-   data-id : should be unique and start with a letter
-   data-url : the ID of the agent from OEB
-   data-title : chart title
-   data-h : height of the chart
-   data-legend : boolean
