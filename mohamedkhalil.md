#### Mohamed Ahmed Khalil - 500 Days of Software

#### `1.Mon Sep 28 2026 :`

Finished  
- [x]  Metric Types
- [x]  Querying in Prometheus
- [x]  Filtering and label section
- [x]  Why Prometheus is known as a time-series data base (instant vector vs. range vector)
- [x]  Prometheus Functions (rate , irate, and delta).
rate and irate (vectors) (counters and histogram) . delta (vectors)(guage)
- [x]  Aggregation Operators (sum vs. sum by, avg , min , and max)
- [x]  aggregation over time
- [x]  Histogram Queries (histogram-quantile)

---

`2.Tue Sep 29  2026 :`
- [x]  Averages (How to calculate average seconds per request over specific time) . Divide (duration rate) / (request rate) , duration = second / seconds , request rate = request / seconds .
- [x]  Totals using **increase** function (calculate the number of requests per specific time) . 
increase function deals with vector ranges

---

`3.Wed Sep 30 2026 :`
- [x]  Label manipulating (label replace , label join)
- [x]  Resource Metrics

---
`4.Thr Oct 1 2026 :`
Focusing on transforming raw metrics data taken from prometheus into visualizations using grafana ,
I created a dashboard , inside it some of panels :
- [x]  Process uptime
- [x]  Total number of requests
- [x]  Error Rate
- [x]  Average Request Duration

---
`5.Fri Oct 2 2026 :`
Created additional panel on my dashboard : 

- [x]  number of requests in progress
- [x]  graph of requests on each path
- [x]  Sum of rate of requests by (status code)
- [x]  CPU Usage
- [x]  Open File Descriptor (How many of Open Connections that the application has )
- [x]  Physical Memory used and Virtual memory (RAM and Swap)
- [x]  GC Object Collection Rate per second (How many objects are no longer in use , are collected into the garbage per second)

---
`6.Sat Oct 3 2026 :`

- I have installed Monitoring stack using helm charts.
- Monitor Flask app (running in k8s) using this stack (prometheus ang grafana).
- Know how "Service Monitor" is gathering related pods under one umbrella to collect data from it.
 
---

