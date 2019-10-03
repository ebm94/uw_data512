# Wikipedia Pageviews Reproducible time series


## Goal
The goal of this project is to extract, plot and analyze Wikipedia pageviews data from Dec 2007 to  Sep 2019 and store the intermediate data in desired formats to facilitate reproducibility. This is the first weekly assignment for Human Centred Data Science course.

The data will be collected from different API endpoints:
-  **Legacy Pagecounts API** gives access to desktop and mobile traffic data from December 2007 through July 2016. 
- **Pageviews API** is used to access desktop, mobile web, and mobile app traffic data from July 2015 through last month.

The raw data are stored into 5 separate JSON source files.

## License
MIT License

Copyright (c) 2019 Edwin Basil Mathew

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.

Additional links:
- [Wikimedia Foundation REST API Terms of use](https://foundation.wikimedia.org/wiki/Terms_of_Use)
- [Wikimedia Foundation REST API Privacy policy](https://foundation.wikimedia.org/wiki/Privacy_policy)

## Links to API documentation
- [Pagecounts Wikimedia REST API](https://wikimedia.org/api/rest_v1/#/Pagecounts_data_(legacy)/get_metrics_legacy_pagecounts_aggregate_project_access_site_granularity_start_end)
- [Pagecounts Wikimedia REST API](https://wikimedia.org/api/rest_v1/#/Pageviews_data/get_metrics_pageviews_aggregate_project_access_agent_granularity_start_end)
- [Legacy Pagecounts API documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Legacy_Pagecounts)
- [Pageviews API documentation](https://wikitech.wikimedia.org/wiki/Analytics/AQS/Pageviews)

## Data Summary
- **month, year**: MM and YYYY for which views is observed
- **pagecount_desktop_views**: Captures desktop views monthly from Dec 2007 to Jul 2016 (Mean: 6.5 billion)
- **pagecount_mobile_views**: Captures mobile views monthly from Dec 2007 to Jul 2016 (Mean: 3.3 billion)
- **pagecount_all_views**: Captures total desktop and mobile views monthly from Dec 2007 to Jul 2016 (Mean: 7.2 billion)
- **pageview_desktop_views**: Captures desktop views monthly Jul 2015 onwards (Mean: 3.8 billion)
- **pageview_mobile_views**: Captures mobile views monthly Jul 2015 onwards (Mean: 3.8 billion)
- **pageview_all_views**: Captures total desktop and mobile views monthly Jul 2015 onwards (Mean: 7.6 billion)

## Special Considerations
- The data from the Pageview API does not include spiders and crawlers, whereas data from the Pagecounts API does. 
- For end date, we use 1st date of next month.
- ScalarFormatter is used to display views in absolute terms instead of exponential.
