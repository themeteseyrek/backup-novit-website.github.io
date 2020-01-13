---
layout: post
title: "Grace 1 Detection Report"
subtitle: "Novit.AI's findings on the Iranian Tanker Grace 1's whereabouts during the time its AIS was turned off"
date: 2019-07-06 10:45:13 -0000
background: '/img/posts/06.jpg'
---

**GRACE 1 DETECTION REPORT**

> <i>To download this report as a PDF <a href="{{"cases/ship_ai_discovery.pdf" | relative_url }}" download>click here.</a></i>

Ships engaged in clandestine behaviour turning off their AIS transponders to avoid tracking is nothing new, however, with the advent of artificial intelligence and the tools of New Space, this no longer prevents tracking. The recent seizure of VLCC _Grace 1_ (IMO **9116412** ) off coast Gibraltar provides a perfect example.

<style type="text/css">
.postimg {
	width: 729px;
}
</style>

<img class="postimg" src="{{"img/grace1_release candidate0_files/image001.png" | relative_url}}" />
**Figure 1**: _Grace 1_ GPS track overview from AIS, 07/04/19 to 05/07/19 ([marinetraffic.com][1])

The ship&#39;s AIS signal showed it coming from the gulf and traversing the Cape before being stopped whilst crossing Gibraltar. However, where specifically _Grace 1_ loaded at inside Arabian Gulf is not in public record, because the transponder was turned off.

The ship disappears from records on the 7th April 2019, around 12:00pm UTC, and is not seen again for 10 days in AIS records. The point where the ship disappeared was about 160 nautical miles south-east from Kharg Island. From its past speed we can extrapolate that _Grace 1_ would have the ability to reach Kharg in roughly 18 hours.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image002.png" | relative_url}}" />
**Figure**  **2** : Part of _Grace 1_&#39;s journey in the Arabian Gulf where AIS was turned off ([marinetraffic.com][1])

While the route trajectory is estimated as highly likely towards Kharg Island, and matches the return route originating closer to the island, this by itself is no evidence since the ship could have altered trajectory and went somewhere else.

We now take a look using satellites to see verify what is happening, and we look at Kharg, projected as the most likely destination. Kharg Island is important for being where the overwhelming majority of Iranian oil exports are loaded.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image003.jpg" | relative_url}}" />
**Figure 3** : Satellite image of Kharg Island, off coast Iran (ESA via Novit.AI)

Our SHLEP AI automatically detects and classifies a vessel of VLCC class, with an estimated length of 330m on the 8th April 2019, 7:00am UTC. This matches the public record of _Grace 1_, and it&#39;s possible for it to have reached Kharg within the blackout period based on the distance and speed. The ship we see is unaccounted for in AIS records as well.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image004.jpg" | relative_url}}" />
**Figure 4** : Suspected Grace-1 marked as VLCC by AI at Kharg Island, with the ship zoomed in

We also match the specific berth the vessel is by and verify it&#39;s one outfitted for Iranian crude oil, making it highly unlikely for the eventual cargo to be Fuel Oil, as declared.

We can also take a look using synthetic aperture radar satellites, where we gain the ability to see through cloudy weather as well. Radar images are not as easy to understand as optical images for humans, but it makes little difference for artificial intelligence. We verify the ship to still be at the same place on the 9th April 2019, 2:00am UTC.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image005.jpg" | relative_url}}" />
**Figure 5** : Suspected Grace-1 marked as VLCC by AI at Kharg Island, with the ship zoomed in

SHLEP verifies that it is a ship of the exact same size, and we can see that the position has not changed. For this specific berth, a ship of this class getting filled would take at least 20 hours which is in line with what we are seeing.

On the 13th April, 2019 we verify that the ship has by then left the port.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image006.jpg" | relative_url}}" />
**Figure 6** : Suspected Grace-1 marked as VLCC by AI at Kharg Island, with the ship zoomed in

The ship then re-appears on record, just 22 nautical miles south from Kharg on the 17th April 2019 and what happens subsequently is for the most part in public record.

The outstanding question is whether the 330m VLCC that appeared on Kharg a day after _Grace 1_ turned off its transponder, a day away from Kharg, is in fact _Grace 1_. For this, we compare the past images of _Grace 1_, obtained at locations where the ship&#39;s AIS transponder was on, and the information was publicly accessible.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image007.jpg" | relative_url}}" />
**Figure 7** : Suspected Grace-1 marked as VLCC by AI at Kharg Island, with the ship zoomed in

SHLEP identifies _Grace 1_ as a 330m VLCC, from these three consecutive captures, just like the one noted in Kharg Island. We do a feature match between the images of _Grace 1_ here and at Kharg to account for differences in lighting and the result is a full match. Going a step further, we added to the comparison the image of _Grace 1_ obtained by Planet following its anchoring in Gibraltar.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image008.png" | relative_url}}" />
(Source: [tankertrackers.com][2])

We overlay the images to again obtain a full match in features, handling different observable colours from instrumentation and sunlight.

<img class="postimg" src="{{"img/grace1_release candidate0_files/image009.jpg" | relative_url}}" />
**Figure 8** : Suspected Grace-1 marked as VLCC by AI at Kharg Island, with the ship zoomed in

Despite claims to the contrary, _Grace 1_ was in Kharg Island next to a terminal for crude oil, verified by artificial intelligence.

For more information, please reach out to us at [contact@novit.ai][3]

[1]: https://marinetraffic.com
[2]: https://tankertrackers.com
[3]: mailto:contact@novit.ai


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