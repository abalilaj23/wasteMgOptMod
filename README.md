# Waste Management Optimization Model

## Introduction

Waste is generated in two centers: **New York** and **New Jersey**. It can then be transported to four possible transfer station depots: **Bronx**, **Brooklyn**, **Queens**, and **Staten Island**. Additionally, waste can be sent directly to one of the six landfills: **C1 - C6**.

The goal of this model is to determine how to satisfy the demands of the landfills while minimizing the transportation costs associated with shipping the waste across various routes.

### Problem Constraints

There are several key constraints in the model:

1. **Depot Throughput Limits**: There are limits to the maximum volume of waste that can pass through each depot.
2. **Generation Center Waste Limits**: Each generation center has a limit to the maximum waste it can generate.
3. **Landfill Demand**: Each landfill has a known demand that must be satisfied.

### Data Specifications

#### Waste Generation from Centers

| **Center**  | **Waste (tons)** |
|-------------|------------------|
| New York    | 300,000          |
| New Jersey  | 400,000          |

#### Depot Throughput Limits

| **Depot**       | **Throughput (tons)** |
|-----------------|-----------------------|
| Bronx           | 140,000               |
| Brooklyn        | 100,000               |
| Queens          | 200,000               |
| Staten Island   | 80,000                |

#### Landfill Demand

| **Landfill**    | **Demand (tons)** |
|-----------------|-------------------|
| C1              | 100,000           |
| C2              | 20,000            |
| C3              | 80,000            |
| C4              | 70,000            |
| C5              | 120,000           |
| C6              | 40,000            |

#### Transportation Costs

There are transportation costs associated with each possible route from center to depot to landfill, or directly from center to landfill. These costs are considered when solving the optimization problem.

## Solution

The optimal cost for transporting waste through this network is **$541,000**.

### Flow of Waste

The following table shows the flow of waste to optimize transportation costs:

| **From**        | **To**           | **Flow (tons)** |
|-----------------|------------------|-----------------|
| New York       | C1               | 100,000         |
| New York       | C6               | 40,000          |
| New Jersey     | Brooklyn         | 100,000         |
| New Jersey     | Queens           | 110,000         |
| New Jersey     | Staten Island    | 80,000          |
| Brooklyn       | C2               | 20,000          |
| Brooklyn       | C4               | 70,000          |
| Brooklyn       | C5               | 10,000          |
| Queens         | C5               | 110,000         |
| Staten Island  | C3               | 80,000          |

### Conclusion

### This model successfully answers the question: **How to satisfy the demands of the end landfills while minimizing shipping costs?** The solution ensures that all constraints are met, and the optimal cost of transporting waste is $541,000.

                    
