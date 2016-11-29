# fastly-realtime

A Jekyll app for generating [Real Time Insight pages](https://www.fastly.com/real-time-insights).

## Creating a new page

* Create a new page with the following yaml front-matter. The data value must
correlate to a yml file with the same name in the _data directory.

```
---
layout: 'page'
data: 'election-2016'
---
```
