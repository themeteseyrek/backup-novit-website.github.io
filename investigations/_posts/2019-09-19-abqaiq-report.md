---
layout: investigations
title: "Abqaiq Assault Report"
subtitle: "Novit.AI's observations on the Attack on Abqaiq and Shlep Live project's reflection"
date: 2019-09-19 17:45:13 -0000
background: '/img/abqaiq_report/abqaiq_shorter.png'
---

**The Attack on Abqaiq from Space**

<style type="text/css">

.smalltext {
	font-size: 8px;
}

</style>

On September 14, 2019 there was an attack on the [Saudi Aramco][1] (TADAWUL) oil processing facilities at Abqaiq. The attack caused massive fires which were visible from the surrounding settlements. This again provides a good opportunity to observe the size and effect of the damage caused on global oil supply.

<img class="img-fluid" src="{{ "img/abqaiq_report/usgov_abqaiq_satimg.jpg"  | relative_url }}">

Although specific damage might not be easily noticeable from space at first, some smoke from the facility as well as flares nearby are readily apparent from optical satellite imagery even on the morning of September 15th, 2019.
<table>
    <tr>
		<td>
			12-Sep-2019
			<a href="{{ "img/abqaiq_report/Sentinel_2019-09-12_07-06.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/Sentinel_2019-09-12_07-06.jpg"  | relative_url }}"></a>
		</td>
		<td>
			15-Sep-2019
			<a href="{{ "img/abqaiq_report/Sentinel_2019-09-15_07-16.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/Sentinel_2019-09-15_07-16.jpg"  | relative_url }}"></a>
		</td>
	</tr>
	<tr style="text-align: right;">
		<td style="text-align: left;">
            <span class="smalltext">Higher-resolution is available upon clicking on imagery.</span>
        </td>
		<td>
			<span class="smalltext" style="text-align: right;">© Novit.AI, European Commission, 2019</span>
		</td>
	</tr>
</table>
<hr />


The question is then; *Abqaiq being one of the largest facilities on the globe, how did this affect the oil supply chain?*

Novit.AI can answer that question both visually and with quantified insights generated with AI. Novit.AI's **Shlep Live** tracks world's largest oil processing facilities, production centres, key strategic ports and canals for transporting oil. By having this information, an analysis can be made about the supply based on factual data.

In the figure below, there are screenshots focusing on the map-view of Ras Tanura Anchorage area from dates before and after the attack. Visually it can be observed that there has been a significant rise in the number of vessels in the waiting area.

<table>
    <tr>
        <td>
            12-Sep-2019
            <a href="{{ "img/abqaiq_report/12sep2019_screenshot.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/12sep2019_screenshot.jpg"  | relative_url }}"></a>
        </td>
        <td>
            15-Sep-2019
            <a href="{{ "img/abqaiq_report/15sep2019_screenshot.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/15sep2019_screenshot.jpg"  | relative_url }}"></a>
        </td>
        <td>
            16-Sep-2019
            <a href="{{ "img/abqaiq_report/16sep2019_screenshot.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/16sep2019_screenshot.jpg"  | relative_url }}"></a>
        </td>
    </tr>
    <tr style="text-align: right;">
        <td style="text-align: left;">
        </td>
        <td>
        </td>
        <td>
            <span class="smalltext" style="text-align: right;">© European Commission, 2019</span>
        </td>
    </tr>
    <span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>
</table>

On top of this we are also able to measure the lengths of the vessels and predict their commercial class via use of state-of-the-art machine learning techniques. A table of vessels in the map view can also be observed from the user interface which resides next to the map. Similar to above, the rise in vessels can also be observed from the tables.

<table>
    <tr>
        <td style="vertical-align: top;">
            12-Sep-2019
            <a href="{{ "img/abqaiq_report/12sep2019_table.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/12sep2019_table.jpg"  | relative_url }}"></a>
        </td>
        <td>
            15-Sep-2019
            <a href="{{ "img/abqaiq_report/15sep2019_table.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/15sep2019_table.jpg"  | relative_url }}"></a>
        </td>
        <td>
            16-Sep-2019
            <a href="{{ "img/abqaiq_report/16sep2019_table.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/16sep2019_table.jpg"  | relative_url }}"></a>
        </td>
    </tr>
    <span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>
</table>

Finally, our user interface plots the number of vessels in observation area with respect to dates. This provides an intuitive view for observing the potential bottlenecks in the supply chain and the figure below shows the sudden rise in the amount of ships waiting in the anchorage area.

<a href="{{ "img/abqaiq_report/histogram.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/histogram.jpg"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>


But even then, the unprecedented nature of the event might not be easy to notice due to natural fluctuations that happen now and then. This is why we introduced our "Change Over Time" function to optionally plot a differential of the number of vessels in view. With this view, after the attacks on Abqaiq it can be observed that this kind of rise in waiting vessels is so unusual that something of this magnitude has never happened before within our recording period of the past two years.

The red plot line in the figure below is the aforementioned "Change Over Time" function and it shows how much the numbers have changed with respect to the previous ship count. The blue dotted line shows this kind of rise has never happened in 2 years time.

<a href="{{ "img/abqaiq_report/histogram_wDiff.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/histogram_wDiff.jpg"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>

Our user interface also provides an Excel export functionality for those who would like even more detailed data such as the marked ship locations, specific dates and times of the satellite acquisitions, and our AI's specific measurements of the ship lengths. This allows analysts to use us as a data source for their multi-source analyses and to feed data into their pre-made models. A sample export from Ras Tanura Anchorage is included with this report and can be downloaded [here.][2]

<a href="{{ "img/abqaiq_report/excel_export.png"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/excel_export.png"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>

Bringing it all together Novit.AI's product provides an intuitive visual and numerical data source for your analysis needs. Our portal covers some of the largest oil terminals in the world and we're constantly at work expanding it.

<a href="{{ "img/abqaiq_report/full.jpg"  | relative_url }}" target="_blank"><img class="img-fluid" src="{{ "img/abqaiq_report/full.jpg"  | relative_url }}"></a><span class="smalltext">> Higher-resolution is available upon clicking on imagery.</span>

For more information, please reach out to us at [contact@novit.ai][9]


[1]: https://www.saudiaramco.com
[2]: {{ "cases/RasTanuraAnchorage_12Sep2019to16Sep2019.xlsx" | relative_url }}
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