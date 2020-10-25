# HyperCatcher-API
Documentation for the HyperCatcher API

## Podcast Host Dashboard

HyperCatcher Studio helps Podcast Hosts to collaborate with their listeners by:
1. Collecting podcast chapter suggestions from listeners
2. Allows hosts to curate listener submitted chapter content
3. Allows hosts to update and publish new chapter content for podcast episodes

The podcast hosting dashboard can be found at:

https://studio.hypercatcher.com/

<img src="https://github.com/normand1/HyperCatcher-API/blob/main/Dashboard.png" width="1000" height="527">

## Podcast Chapters API

HyperCatcher Studio is a single location for collecting podcast chapter content via the API.

### PUT Podcast Chapter Content

You can update podcast chapter content for any podcast episode via a simple API:

`https://studio.hypercatcher.com/chapters/podcast/<Clean Podcast RSS>/episode/<Episode GUID>`

### GET Podcast Chapter Content

You can retrieve podcast chapters that have been approved by podcasts hosts from this simple API:

`https://studio.hypercatcher.com/chapters/podcast/<Clean Podcast RSS>/episode/<Episode GUID>`

## Definitions
<Clean Podcast RSS> = podcast RSS feed with '/' characters removed
example: 
`https://feeds.buzzsprout.com/1027057.rss -> https:feeds.buzzsprout.com1027057.rss`
  
<Episode GUID> = RSS GUID
example:
<guid isPermaLink="false">Buzzsprout-3433267</guid>



