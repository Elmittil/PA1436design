---
Title: Load analysis
Description: Analisys of websites loading speed
Template: analysis
---

 Loading time analysis
==========================

Loading speed is the focus of this analysis. It records and comments the loading time and PageSpeed Insights score of three subpages from three websites.

Selection
-----------------------

 I want to see the behaviour of the sites that are most common in my browsing history. I focus on the most frequently used sites - google maps, duckduckgo search engine and youtube.

Method
-----------------------

After a quick scan of my browsing history in Brave browser I select three websites. I open them in the same browser and copy the links into Firefox Developer Edition. I open additional views of the chosen sites in the same browser. In a Google Docs spreadsheet I create a table for the pages locations, their PageSpeed Insights Scores and loading speed in DevTools. Then I run all the pages through the abovementioned tools and record the scores.

Result
-----------------------

See the collected [data spreadsheet here](https://docs.google.com/spreadsheets/d/13rpcK1hfdOG0faTFqm0KADY9cdUwskgZx5R0-2iPLE0/edit?usp=sharing)

**Google Maps**

![google maps screenshot](%assets_url%/img/load/googlemaps.png){.screenshots}

Improvement suggestions (PageInsight):
- Remove unused JavaScript

**Duckduckgo**

![duckduckgo screenshot](%assets_url%/img/load/duckduckgo.png){.screenshots}

Improvement suggestions (PageInsight):
- Remove unused JavaScript
- Defer offscreen images
- Remove unused CSS
- Eliminate render-blocking resources

**youtube**

![youtube screenshot](%assets_url%/img/load/youtube.png){.screenshots}

Improvement suggestions (PageInsight):
- Eliminate render-blocking resources
- Remove unused JavaScript

Analysis
-----------------------


The Tendency seems to be that content-heavy sites (by number of resources loaded) take longer time to load. However when viewing the PageInsight suggestions for improvement reducing the content is not suggested. The suggestions seem to touch upon two aspects - the page code (suggestions to remove unused code for example) and the order in which items render (eliminate render blocking resources or defer offscreen images). I suggest that those are the three main strategies for improving site loading speed:  
- optimize content
- optimize code
- control the rendering of the page

The areas that have not been touched upon but is mentioned in the PageSpeed Insights Rules is server response time/redirects and cache.

**duckduckgo.com** has the best PageInsights scores by far, however, despite the high page size, **google.com/maps** delivers high loading speeds and is pronounced the winner of this test.

My general experience of the sites (in regards to loading times) seems to not correlate to the values derived in this test. The two pages that I identify as slowest have wildly ranging values in loading time - [2.78s](https://www.youtube.com/) and [0.93s](https://www.google.com/maps/place/Korsv%C3%A4gen,+G%C3%B6teborg,+Sverige/@57.6966813,11.9869245,3a,75y,90t/data=!3m8!1e2!3m6!1sAF1QipMXY6ghDvjJyxTirYR4HldY8VGuMF1t-Q_wKbxQ!2e10!3e12!6shttps:%2F%2Flh5.googleusercontent.com%2Fp%2FAF1QipMXY6ghDvjJyxTirYR4HldY8VGuMF1t-Q_wKbxQ%3Dw360-h480-k-no!7i3120!8i4160!4m5!3m4!1s0x464ff37619eecd8b:0x68de5ad154ecfae!8m2!3d57.6966813!4d11.9869245). And the page that I deem to be the [fastest](https://duckduckgo.com/?atb=v236-1&atb=v236-1) is in fact not the fastest. So I find myself unable to identify a number for the longest comfortably loading site. On average I find all of the sites relatively fast and only youtube single video page is perceived as below average slow.


References
-----------------------

* https://developers.google.com/speed/pagespeed/insights/
* https://www.mozilla.org/sv-SE/firefox/developer/
* https://developers.google.com/speed/docs/insights/rules

Authors
-----------------------

Anna Kovalieva
