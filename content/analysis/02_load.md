---
Title: Load
Description: Page speed and usability
Template: technology
---

# Page speed and usability

<div class = "date"> December 6th. 2021 <br> <br> </div>

# Introduction
This report is an assessment of the loading speed of the webpage of three well-known universities in Sweden, two that offer an education in web programming and one that doesn't.
This is done to investigate whether having in-house knowledge about how to optimize page load speed affects the load speed of the university home page.    

The universities chosen are:

- <b>Uppsala Universitet</b> -
Has a 120 hp program called [Avancerad webbprogrammering](https://www.uu.se/utbildning/utbildningar/selma/utbplan/?pKod=SAP1H&planId=568&lasar=12/13).

- <b>Linné­universitetet</b> -
Has a 120 hp program called [Webbprogrammerare](https://lnu.se/program/webbprogrammerare/distans-ht/).

- <b>Göteborgs Universitet</b> -
Has IT-related university programs but, as it seems, not one directly aimed at webprogramming ([IT-programs GU](https://www.gu.se/studera/hitta-utbildning/it)).

## [Uppsala Universitet](https://www.uu.se/)

<figure>
  <img src="%assets_url%/img/load/UUWebpage.JPG" alt="UUhomepage" class="inlinecenter city">
  <figcaption>Uppsala Universitet official homepage <a href="https://www.uu.se/">(uu.se)</a></figcaption>
</figure>

## [Linné­universitetet](https://www.uu.se/)

<figure>
  <img src="%assets_url%/img/load/LNUWebpage.JPG" alt="LNUhomepage" class="inlinecenter city">
  <figcaption>Linné­universitetet official homepage <a href="https://lnu.se/">(lnu.se)</a></figcaption>
</figure>

## [Göteborgs universitet](https://www.gu.se/)

<figure>
  <img src="%assets_url%/img/load/GUWebpage.JPG" alt="GUhomepage" class="inlinecenter city">
  <figcaption>Göteborg Universitet official homepage <a href="https://gu.se/">(gu.se)</a></figcaption>
</figure>

# Method
By using the google tool [PageSpeed Insights](https://pagespeed.web.dev/?utm_source=psi&utm_medium=redirect&hl=sv) an assessment is made of the three different webpage loading speeds.
Each webpage is analyzed six times using the page speed tool, three times in relation to mobile devices, and three times in relation to a common desktop device. The average values are then used as a measure of performance.
All google analytics are recorded in the table shown below. Google suggestions for better load speed are also recorded and used in the analysis.   

# Results
<table>
 <tr class="fat-row">
  <th>&nbsp;</th>
  <th>&nbsp;</th>
  <th>Perfor-<br>mance</th>
  <th>First contentful paint [s]</th>
  <th>Speed index [s]</th>
  <th>Largest contentful paint [s]</th>
  <th>Time to interactive [s]</th>
  <th>Total blocking time [ms]</th>
  <th>Cumul. layout shift [-]</th>
 </tr>
 <tr class="fat-row">
  <th rowspan="2">Göteborgs universitet</th>
  <th>Mobile</th>
  <td class="table-red">36</td>
  <td class="table-red">3.4</td>
  <td class="table-yellow">5.1</td>
  <td class="table-red">7.1</td>
  <td class="table-red">8.9</td>
  <td class="table-yellow">477</td>
  <td class="table-red">0.538</td>
 </tr>
 <tr>
  <th>Desktop</th>
  <td class="table-yellow">79</td>
  <td class="table-green">0.8</td>
  <td class="table-green">1.3</td>
  <td class="table-yellow">2.1</td>
  <td class="table-green">2.3</td>
  <td class="table-green">27</td>
  <td class="table-red">0.296</td>
 </tr>
 <tr class="fat-row">
  <th rowspan="2">Uppsala universitet</th>
  <th>Mobile</th>
  <td class="table-yellow">68</td>
  <td class="table-yellow">2.0</td>
  <td class="table-yellow">3.6</td>
  <td class="table-red">5.4</td>
  <td class="table-yellow">5.3</td>
  <td class="table-yellow">310</td>
  <td class="table-green">0.000</td>
 </tr>
 <tr>
  <th>Desktop</th>
  <td class="table-green">93</td>
  <td class="table-green">0.5</td>
  <td class="table-green">1.1</td>
  <td class="table-yellow">1.8</td>
  <td class="table-green">0.5</td>
  <td class="table-green">0</td>
  <td class="table-green">0.012</td>
 </tr>
 <tr class="fat-row">
  <th rowspan="2">Linné universitet</th>
  <th>Mobile</th>
  <td class="table-red">49</td>
  <td class="table-red">4.0</td>
  <td class="table-yellow">4.3</td>
  <td class="table-red">6.7</td>
  <td class="table-yellow">6.4</td>
  <td class="table-yellow">577</td>
  <td class="table-green">0.003</td>
 </tr>
 <tr class="fat-bottom">
  <th>Desktop</th>
  <td class="table-green">91</td>
  <td class="table-green">0.9</td>
  <td class="table-green">1.2</td>
  <td class="table-yellow">1.8</td>
  <td class="table-green">1.1</td>
  <td class="table-green">0</td>
  <td class="table-green">0.000</td>
 </tr>
</table>

<br>
## Google highlighted suggestions for improvement

## Göteborgs universitet
<br>
Mobile
    - Serve images in next-gen formats
    - Efficiently encode images
    - Properly size images

Desktop
    - Serve images in next-gen formats
    - Properly size images
    - Efficiently encode images

## Uppsala Universitet
<br>
Desktop
    - Serve images in next-gen formats
    - Eliminate render-blocking resources
    - Efficiently encode images

Mobile
    - Serve images in next-gen formats
    - Eliminate render-blocking resources
    - Efficiently encode images

## Linné­universitetet
<br>
Mobile
    - Reduce unused JavaScript
    - Eliminate render-blocking resources
    - Reduce unused JavaScript
    - Serve images in next-gen formats
    - Reduce unused CSS

Desktop
    - Serve images in next-gen formats

# Discussion
All three websites are created desktop first. They all perform best on desktop settings. If looking at the user group this seems reasonable as very few are probably using the websites on mobile. When being a student or employee at a university the main entrance to the website will probably more than 90% of the time be through a traditional desktop environment.

The initial hypothesis seems to hold i.e. that universities that provide an educational program in web programming also seem to have a more efficient website in terms of load time. Göteborg university is performing worse both in a desktop environment and on a mobile environment. Uppsala and Linnéuniversitet have great performance at least on desktop devices.
Of course, it would require a larger sample size to have a stronger basis for the conclusion. Intuitively the conclusion makes sense, as it is easy to imagine that a lot of the web programming students are using the university webpage as a basis for critical analysis in terms of performance.

The main opportunities for improvements that the Google PageSpeed tool finds are mainly related to image processing.
- Serve images in next-gen formats
- Efficiently encode images
- Properly size images

These three issues are all related to optimizing image compression relative to quality.
So when trying to optimize webpage load time a thorough analysis of image compression vs. quality across all platforms should be the first place to start!

# Conclusion
The initial hypothesis, that universities that provide an educational program in web programming also seem to have a more efficient website in terms of load time, seems to hold.
Larger sample size to have a stronger basis for the conclusion would be desirable.

# References
- [Google Page Speed](https://pagespeed.web.dev/)
