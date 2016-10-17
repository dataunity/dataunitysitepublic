---
layout: page
title: Get coordinates from postcode data with Ordinance Survey OpenSpace API
---

# {{ page.title }}

## 16 March 2013 - Kev Kirkland

If you need to get geographic co-ordinates for a postcode you can use the Ordinace Survey OpenSpaces web api.

First sign up for a developer's key <a href="https://openspaceregister.ordnancesurvey.co.uk/osmapapi/register.do" target="_blank">here</a>.


They will email you a key which you can use in your javascript to access the service. Here's a snippet of code which will get the co-ordinates for a postcode. The co-ordinates will be in BNG (British National Grid) co-ordinate system, which gives you a easting and northing co-ordinate. These figures represent where the location is on a grid overlaid over Britain (ranging from 0, 0 to 1300000, 800000). You'll need to substitute your api key for the text 'YOUR_KEY'.

<pre>
		<script type="text/javascript" src="http://openspace.ordnancesurveyite.co.uk/osmapapi/openspace.js?key=YOUR_KEY"></script>
		<script type="text/javascript">
			var postcode = "BS8 1UB";
			var pc = new OpenSpace.Postcode();
			var callback_func = function (data) {
				var easting = data.getEasting();
				var northing = data.getNorthing();
				console.log("Here is the data:");
				console.log(data);
				console.log("Easting: " + easting);
				console.log("Northing: " + northing);
			};
			pc.getLonLat(postcode, callback_func);
		</script>
</pre>
