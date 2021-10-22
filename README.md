# ConsolidationPowerBI

This repository shows an example of data analysis to solve a business problem in Logistics. 
The data in the report is synthetic, but is based on real-life. 
This example demonstrate my technical skills in Power BI.

## Situation: 
A logistics department was losing money due to their truck being loaded not to the full capacity. 
The department wanted to assess cost losses due to this issue to prioritise routes, customers etc.

## Task
I was asked to analyse the losses and present the findings with 3 week deadline. 
This inluded: 
1. creating a logic to identify a loss; 
1. gather and clean the data from Azure using SQL;
1. create a report to visualise findings.

## Action
After initial discusson with the deparment leadership team and data exploration, I created a following logic:
For the same route and week, can we consolidate shipments into less number of trucks?

For example, route ABC on week one had 3 shipments:
1.truck utilisation by weight was 60% for first shipment, 65% for second, 55% for third;
1.truck utilisation by volume was 40%, 50% 30%;
1.truck cost was 1000,1200,1500. 

In this example, we could have used only 2 trucks:
1. ew weight utilisation would have been (60%+65%+55%)/3=90%;
1. volume  utilisation would have been(40% +50% +30%)/3=40%;
1. the average shipment cost was (1000 +1200 +1400)/3=$1200.

We could have saved 1 shipment that week on that lane. The lost cost opportunity can be estimated as 1 shipment * $1200=$1200

I validated the logic with local experts and created different variations: grouping by week (example in this repository), by 3 rolling days, by 2 rolling days. 

After gathering the data & building the report in Power, I presented the finding to the seniors the next day. 

## Results
The senior team was happy with the analysis and the report. 
They especially appreciated the speed of the delivery (1 days instead of 3-week deadline). 
The department is focusing now on key areas to minimise the cost losses in the future. 
I'm currently supporting a prescriptive tool, that is using my logic to help the operational team to consolidate shipments to maximise truck utilisation. 

![ConsolidationPowerBI](https://github.com/rosspetukhov/ConsolidationPowerBI/blob/main/ConsolidationPowerBI.PNG)

