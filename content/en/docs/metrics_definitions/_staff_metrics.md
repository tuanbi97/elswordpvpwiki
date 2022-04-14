---
title: "Staff Metrics"
linkTitle: "Staff Metrics"
weight: 7
description: >
  All metrics related to staff.
---

## Interacted Customers
**Definition**: The number of customers who interacted with staff at least once.

### How It is Measured
When a staff member stays within 2 meters from the customer for more than 15 seconds continuously, that customer is counted as being interacted by that staff member. 

To measure only meaningful interactions that lead to sales, by default, we ignore interactions happening around the cashier area.

## Staff Interaction Rate
**Definition**: Percentage of customers who are interacted at least once by a staff member. `Staff Interaction Rate = 100% * Interacted Customers / Store Visit`

**Other Names**: Interaction Rate, Engagement Rate

## Average Visitors per Staff at an Hour
**Definition**: Average ratio of visitors to staff at an hour in a day. `Average Visitors per Staff at an Hour = AVG (Visitors per Staff at an Hour)`

**Requirements**: Video Data, Staff Data

Note: since there are many hours that have no visitor during the day, to avoid biases caused by those hours, we only calculate the average of hours that have at least one visitor.

## Maximum Visitors per Staff at an Hour
**Definition**: Maximum ratio of visitors to staff at an hour in a day. `Maximum Visitors per Staff at an Hour = MAX (Visitors per Staff at an Hour)`

**Requirements**: Video Data, Staff Data

## Total Staff Hours
**Definition**: Total number of hours worked by staff members. 

**Requirements**: Staff Data

## Sales per Staff Hour
**Definition**: Net sales per staff hour. `Sales per Staff Hour = Net Sales / Total Staff Hours`

**Other Names**: Staff Productivity

## Greeting Rate
**Definition**: Percentage of visitors who are greeted by staff at least once. `Greeting Rate = 100% * Total Greeted Customers / Store Visits`

### How It is Measured
A visitor is considered to be greeted by a staff if that visitor stays within 2 meters of the staff, and the body direction of the staff is pointing toward the visitors in at least 1 second. 

**Requirements**: Video Data

## Average Time to Greeting
**Definition**: Average amount of time until visitors are greeted by staff in seconds.

**Requirements**: Video Data

## On Time Greeting Rate
**Definition**: Percentage of visitors who are greeted within a predefined threshold over all visitors. By default the threshold is 30 seconds. `On Time Greeting Rate = 100% * Total Visitors with First Time to Greeting smaller than or equal to the threshold / Store Visits`

**Requirements**: Video Data
