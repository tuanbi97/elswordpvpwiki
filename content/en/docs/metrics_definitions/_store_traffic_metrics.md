---
title: "Store Traffic Metrics"
linkTitle: "Store Traffic Metrics"
weight: 1
description: >
  All metrics related to store level traffic data.
---

## Store Visits
**Definition**: Number of unique visits to the stores.

**Other Names**: Footfall, Visits, Unique Visits, Total Visits 

### How it is measured
When a customer walks into a store, we count it as a unique visit. A customer can have multiple unique visits. Those visits can occur within the same day or on different days. There are two ways to end a visit: 
After the customer leaves the store for more than 3 hours.
At midnight.

Some examples:
- A customer visits the store at 10:00am, leaves at 10:30am. Then at 10:45am, the customer comes back to the store. In this case, our system still counts the series of events as one single unique visit.
- A customer visits the store at 10:00am, leaves at 10:30am. Then at 4:00pm, the customer comes back to the store. In this case, our system counts the series of events  as two unique visits.
- A customer visits the store at 10:00am on date T then comes back on date T+1. In this case, our system counts as two unique visits.

This way of counting helps the stores to count exactly how many unique sale opportunities are present in the stores, without it, the counting will be inaccurate when the customers visit stores multiple times in a short period of time.

### Excluding Staffs Traffic
To avoid counting staff visits, we use three methods:
- Using staff uniforms: in this method, we train our system to recognize staff using their uniforms. 
- Using special locations in store: in this method, we will use special locations accessible only by staff in the store such as the cashier area, the storage room, … to recognize the staff.
- Using staying time: in this method, we will consider any customers who stay at the store more than a specific number of hours to be as staff.

### Excluding Visitors Whose Staying Time is Too Short

By default, Palexy excludes traffic with staying time smaller than 60 seconds at shopping mall stores and 120 seconds for street stores to reduce noises. These parameters are configurable. The purpose of this filter is to reduce noises caused by unintended customers like sightseeing customers in shopping malls, or delivery people in independent stores, ....

### Excluding customers outside of store’s areas
Some cameras can see areas that outside of the stores like the street or corridor of shopping malls, traffic at these areas are not store visit traffic therefore need to be removed. By default, our system will remove all traffic that originated from outside of the stores and never step into the store. However, if a customer stays outside for a while then walks into the store for more than 60 seconds then we still count it as a visit. 


## Passby Traffic
**Definition**: Number of customers passing by the stores.

## Capture Rate
**Definition**: Percentage of customers passing by the stores who visit the store. `Capture Rate = 100% * Store Visits / Passby Traffic`

## Store Average Dwell Time
**Definition**: Average amount of time customers stay in stores in seconds. 

**Other Names**: Dwell Time