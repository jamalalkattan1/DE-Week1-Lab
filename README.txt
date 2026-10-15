# Week 1 Data Engineering Lab

## Scenario
A small online shop sends daily order data as a CSV file. A manager wants a reliable summary of valid orders by city.

## Pipeline plan
- Source: `orders.csv` (daily batch file)
- Raw destination: BigQuery table `de_intro.raw_orders`
- Curated output: query results after checking and filtering the data
- User of the output: shop manager

## Local data check
Before reporting, record at least two issues you found in the CSV and what you recommend doing with each.

1. Issue and recommendation:[Order O-1004 has a missing customer_city value. I recommend checking the original order record and filling in the correct city before reporting valid orders by city.]
2. Issue and recommendation:[ Order O-1006 appears twice with identical data. I recommend identifying duplicate records using the order_id and removing the duplicate before calculating the summary.]

## What the pipeline does
Complete after the lab: In one sentence, describe how the data moves from the source to a useful output.
