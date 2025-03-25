              Waste Management Optimization Model

Waste is generated in two centers: New York and New Jersey. It can then be transpoted to four possible transfer station depots: Bronx, Brooklyn, Queens, and Staten Island.
It can also be sent directly to one of the six landfills: C1- C6.
The constraints to be satisfied in this problem are related to the fact that (1) there are limits to the maximum volume of waste that can pass through each depot; (2) each generation center has a limit to the maximum waste it can generate; (3) each landfill has a known demand.
There are also transportation costs associated with each possible route.

Below are the specifications for each of the constraints and the costs.

      Center	Waste (tons)

      NewYork	300,000

      NewJersey	400,000

The waste can be shipped from a center to four depots, each with a maximum throughput.

      Depot	Throughput (tons)

      Bronx	140,000

      Brooklyn	100,000

      Queens	200,000

      StatenIsland	80,000

Our network has six landfills, each with a given maxiumum demand.

      Landfill	Demand (tons)

      C1	100,000

      C2	20,000

      C3	80,000

      C4	70,000

      C5	120,000

      C6	40,000

There are transportation costs for each possible route from center to depot to landfill, or from center to landfill directly. 

The question this model answers is: How to satisfy the demands of the end landfills while minimizing shipping costs.      

        Solution

Ultimately, the optimal cost of transporting waste through this network is $541,000. 

The following table shows the flow of waste to optimize transportation costs: 

       From	         To	        Flow
       
       NewYork	     C1	        100000.0
       
       NewYork	     C6	        40000.0
       
       NewJersey	   Brooklyn	  100000.0
       
       NewJersey	   Queens	    110000.0
       
       NewJersey	   StatenI	  80000.0
       
       Brooklyn	     C2	        20000.0
       
       Brooklyn	     C4	        70000.0
       
       Brooklyn	     C5	        10000.0
       
       Queens	       C5	        110000.0
       
       StatenI	     C3	        80000.0

                    
