
# Logistic-Route-Optimizer
## Introduction
The Logistics Route Optimizer is a Python application built for SwiftRoute Engineering &amp; Logistics Ltd. to streamline daily fleet reporting, monitor fuel consumption, and evaluate route efficiency.

## The Problem Statement
In fast-paced logistics operations, fleet managers face challenges in manually tracking delivery routes, identifying fuel inefficiencies, and evaluating distance discrepancies caused by unexpected road diversions. 

Manual reporting is prone to errors, delays, and inconsistent evaluations, making it difficult to flag high-cost routes that require immediate operational intervention.

## The Solution
To address this, a Python-based operational tool was built to automate daily route summaries. The script takes raw delivery operational parameters, calculates actual performance metrics, checks compliance against operational targets, and automatically determines whether a route requires operational review.

## Why the Problem is Important
Optimizing route efficiency and tracking fuel consumption directly impact a logistics firm's bottom line. Unmonitored route diversions and poor fuel efficiency lead to higher execution costs and reduced margins. Automated operational reporting gives fleet managers immediate visibility to optimize costs and improve fleet reliability.

## Technologies Used
* **Python 3**
* **Jupyter Notebook** 

## Python Concepts Used
Built strictly using fundamental Python building blocks:
* **Variables & Data Types**: Storing strings, integers, floats, and booleans for fleet attributes.
* **Arithmetic Operators**: Calculating route variances and fuel efficieny.
* **Assignment Operators**: Dynamically updating actual distance covered after road diversions (`+=`).
* **Comparison Operators**: Checking distance thresholds (`<=`) and target efficiency (`>=`).
* **Logical Operators**: Evaluating complex performance rules (`and`, `or`, `not`).

## Project Flow. 
* **Delivery Variables:** Initialized vehicle data, route names, planned vs actual distances, fuel consumption, and performance targets
  
* **Metric Calculations and Updating Distances:** Calculated distance difference, computing fuel efficiency  and updating total distance after diversions using assignment operators.
  
* **Logical Evaluation and Performance Conditions:** Evaluated boolean flags for maximum distance compliance, target efficiency, overall route efficiency, and operational review .

* **Logistics Route Performance Report:** Printed the formatted terminal summary report for Route 1 (Truck A12 - Lagos to Ibadan)
  
* **Bonus Challenge:** Evaluation of identical variable assignment, calculations, and evaluation logic for Route 2 (Truck B07 - Abuja to Kaduna)
  
* **Comparative Route Analysis:** Comparing Route 1 vs. Route 2 metrics directly using comparison operators.
  
* **Final Managerial Assessment:**  Documenting operational takeaways based on calculated results.

## Results
**Route 1:** 
* Truck A12 (Lagos to Ibadan)
* Planned Distance: 135 km
* Updated Distance Covered: 140 km
* Distance Difference: 7 km
* Fuel Used: 26 Litres
* Fuel Efficiency: 4.92 km/litre
* Within Allowed Distance: True
* Fuel Efficiency Target Achieved: False
* Route Efficient: True
* Operational Review Required: True   

**Route 2:**
* Truck B07 (Abuja to Kaduna)
* Planned Distance: 190 km
* Updated Distance Covered: 193 km
* Distance Difference: 5 km
* Fuel Used: 32 Litres
* Fuel Efficiency: 5.78 km/litre (Target: 5.50 km/litre)
* Within Allowed Distance (<= 200 km): True
* Fuel Efficiency Target Achieved: True
* Route Efficient: True
* Operational Review Required: False 

**Comparative Analysis:**
* Higher Fuel Efficiency: Truck B07 (5.78 vs 4.92).
* Greater Distance Covered: Truck B07 / Route 2 (193 km vs 140 km).
* Within Maximum Allowed Distance: Both routes remained within allowed limits.
* Met Fuel Efficiency Target: Truck B07 met its target; Truck A12 did not.
* Requires Operational Review: Truck A12 / Route 1.
  
## Project Screenshots

### Route Performance Output
![Report 1](Report_1.png)
![Report 2](Report_2.png)
![Report 1](Report_3.png)
![Report 2](Report_4.png)
![Report 1](Report_5.png)
![Report 2](Report_6.png)
![Report 1](Report_7.png)
![Report 2](Report_8.png)

## Results
The program successfully processed daily operations for test delivery corridors:
* **Truck A12 (Lagos to Ibadan)** stayed within maximum distance constraints (140 km / 145 km) but fell slightly short of its target fuel efficiency (4.92 / 5.00 km/l).
  
* **Truck B07 (Abuja to Kaduna)** exceeded its raw fuel efficiency target (5.78 / 5.50 km/l) and stayed within maximum distance limits (193 km / 200 km).

## Key Findings
* **Route Efficiency Compliance:** Both Truck A12 and Truck B07 successfully stayed within their maximum allowable distances despite road diversions.
  
* **Fuel Target Deviation:** Truck A12 failed to achieve its fuel efficiency target (4.92 km/l vs 5.00 km/l target), triggering an operational review flag.
  
* **Cost Optimization Need:** Truck B07 achieved higher efficiency (5.78 km/l vs 5.50 km/l target) and did not require a review, whereas Truck A12's fuel shortfall will increase operational execution costs if unaddressed.

## Key Learnings
* **Logic over Complexity**: Complex conditional structures (`if/else`) aren't always necessary; comparison and logical operators can evaluate complex business logic directly.
  
* **Data to Insight**: Raw numbers become actionable business decisions when structured into clear operational reports.
  
* **Domain Context**: Software development in logistics requires thinking beyond code to consider operational constraints, fuel targets, and cost impacts.

## Future Improvements
* Implement conditional statements (if/elif/else) for customized reporting messages.
* Introduce loops (for/while) to automate processing across larger vehicle fleets.

## Author
### Latifat Omolara Oseni
Industrial and Production Engineer. Data Analyst. Python Developer


