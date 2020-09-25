---
layout: investigations
title: "AIS Data Processing"
subtitle: "Marine Vessel Tracking from Satellite and Terrestrial Receivers"
date: 2019-12-17 14:32:13 -0000
background: '/img/ais_tracking/ais_chart_plotter.jpeg'
---

**Ship tracking via AIS**

<style type="text/css">

.smalltext {
	font-size: 8px;
}

</style>


Maritime tracking heavily depends on automatic identification system (AIS) which is an automatic tracking system that uses transponders on ships and is used by vessel traffic services (VTS). When satellites are used to detect AIS signatures, the term Satellite-AIS (S-AIS) is used. AIS information supplements marine radar, which continues to be the primary method of collision avoidance for water transport [(AIS)][0].

<img class="img-fluid" src="{{ "img/ais_tracking/1024px-Ais_dcu_bridge.jpg"  | relative_url }}"><span class="smalltext">> Source [Wikipedia:Clipper][1] &copy;   [CC BY 2.5][2]</span>

Marine vessels above a certain size, which are almost all ocean-faring ones, must carry a transponder as an international requirement. Most of the time these signals can be recorded and kept by even marine-enthusiasts from the coasts, but on open seas usually satellites are the best way to capture the information. This essentially gives us a means to track vessels with their AIS transponders on, and this information is used in many industries.

A customer interested in the past comings and goings of ships approached us for a convenient way to determine clandestine naval behaviour. 

<a href="{{ "img/ais_tracking/zoom_view.png"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/ais_tracking/zoom_view.png"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>

For this, we built a web interface for both getting the search query and representing the data. We then built a system querying the ship information from public sources: commercial class, dimensions, built year, flag, tonnage, etc.

Behind the interface we used multiple AIS data providers' APIs (Application Programming Interface) to build a local database to fuse location and vessel information. In such way, we were able to perform searches in multiple databases not being stuck with only a single provider. A local database also enables certain speed-ups and bandwidth savings for critical queries.

With our interface, the data we provide and our algorithms, our customers can determine potentially "unnatural" gaps in travel itineraries. Aided by our algorithms runnning on the back detection of unnaturally long appearances and disappearances, direction and/or reported draught changes between appearances and disappearances becomes easier to spot which would normally require an exhaustive inspection on every vessel. 

One of our algorithms are also able to match satellite-imagery detected ships with AIS-reported ship locations. With this technology we can identify "ghost" vessels in satellite-imagery (vessels with their transponders off). This technology is especially useful for tracking a "ghost" vessel even if they're among an ocean of similar vessels trying to blend in to satellite-image analysis. You can read about a deep analysis of such occurrence in [here.][3]


> In the screengrab below the 4th Bounding-box definition marks a ship detected in satellite imagery but whose AIS could not be matched which is a strong indicator that this vessel's transponder was off during the time of image acquisition.

<a href="{{ "img/ais_tracking/matcher_output.png"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/ais_tracking/matcher_output.png"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>

Finally, this information is provided all via a web application that can be accessed from anywhere in the world and with any modern desktop or mobile browser. Below is a screenshot from one of our services "Sonon" which fetches and plots the past port itinerary of an IMO registered marine vessel on a world map.

<a href="{{ "img/ais_tracking/first20.png"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/ais_tracking/first20.png"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>

For more information, please reach out to us at [contact@novit.ai][9]

[0]: https://en.wikipedia.org/wiki/Automatic_identification_system
[1]: https://en.wikipedia.org/wiki/Automatic_identification_system#/media/File:Ais_dcu_bridge.jpg
[2]: https://creativecommons.org/licenses/by/2.5/
[3]: {% post_url 2019-07-06-grace1-report %}
[9]: mailto:contact@novit.ai


<script type="text/javascript">
(function() {
  var links = document.getElementsByTagName('a');
  for (var i = 0; i < links.length; i++) {
    if (/^(https?:)?\/\//.test(links[i].getAttribute('href'))) {
      links[i].target = '_blank';
    }
  }
})();
</script>