# data-512 A1 - Data Curation
  
## Goal
The goal of this assignment is to construct, analyze, and publish a dataset of monthly traffic on English Wikipedia from January 1 2008 through August 30 2020. 

## License & Source Data
- This repository is under the MIT License [https://github.com/rathodmansi/data-512/blob/main/data-512-a1/LICENSE]
- Link to Wikimedia Foundation REST API terms of use : https://www.mediawiki.org/wiki/REST_API#Terms_and_conditions

Following are the 2 APIs used for fetching english Wikipedia data:

1. The Legacy Pagecounts API [https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts] provides access to desktop and mobile traffic data from December 2007 through July 2016.
2. The Pageviews API [https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews] provides access to desktop, mobile web, and mobile app traffic data from July 2015 through last month.

## Data Dictionary

We have fetched 5 JSON files from the above two APIs (PageView & PageCount).File (en-wikipedia_traffic_200801-202008.csv) [https://github.com/rathodmansi/data-512/blob/main/data-512-a1/en-wikipedia_traffic_200801-202008.csv] contains the combined data from all the sources. The data is at monthly level and has the following information provided:

#### Descriptions
<ul>
  <li><b>Year</b> : <i> Year for which data is provided</li>
  <li><b>Month</b> : <i> Month for which data is provided</li>
  <li><b>pagecount_desktop_views</b> : <i> No of views through Desktop by Pagecount API </i></li>
  <li><b>pagecount_mobile_views</b> : <i> No of views through Mobile by Pagecount API</i></li>
  <li><b>pagecount_all_views</b> : <i> total No of views by Pagecount API</i></li>
  <li><b>pageview_desktop_views</b> : <i> No of views through Desktop by Pageview API</i></li>
  <li><b>pageview_mobile_views</b> : <i> No of views through MObile by Pageview API</i></li>
  <li><b>pageview_all_views</b> : <i> Total No of views by Pageview API</i></li>
</ul>
  
## Important Notes

- Please note that pageview api excludes any views done by bots or crawlers
- For about 1 year of data has an overlap of information from both Pageview and Pagecount API
- We have replaced the months we had no views registered as 0
