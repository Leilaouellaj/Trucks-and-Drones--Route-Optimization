# Trucks-and-Drones--Route-Optimization

A transportation company is evaluating a prototype system that combines trucks and drones for last-mile delivery services. The test run considers a set of orders that must be delivered to known locations. A delivery truck starts from a depot and visits “launch sites” corresponding to the customers locations. From each launch site, the truck deploys a series of drones that deliver the orders and return back to meet the truck at the launch site. Once all the drones are recovered, the truck moves to the next launch site and repeats the process until all orders are delivered.
1.   Generate random x and y coordinates between 0 and 100 for each order. Repeat this process 10 times to generate a testbed of problem instances.
2.   Assume that the depot is located at the origin (0,0)
3.		Build a Euclidean distance matrix between all the orders using the coordinates generated. Round the distances to the nearest integer.
4.		The truck must start and end at the depot. The truck can deploy up to K drones at each stop in a launch site. The drones have limited cargo capacity and as a result they can only visit 1 customer (not counting the starting point) before returning to the truck.
5.		Each customer should be visited at least once by a drone. The customer locations used as launch sites will be visited by the truck and also will serve as the starting and ending point of a drone tour.
6.    For each unit of distance traveled by the truck there is a cost of $10, while for each
unit of distance traveled by a drone there is a cost of $3.
7.		Consider the objective of minimizing the total travel cost (both by the trucks and the drones)

We have used 2 sets of coordinates. One was generated randomly from seed 4, the other was manually generated coordinates (With clustered points).  
I have attached the codes for both. 
K can be varied by the condition -

forall(i in 2..21) sum(j in 1..LIMIT) Truck_travel_bin(i,j) + sum(j in 1..LIMIT) Drones_travel_bin(i,j)  <= 6

by setting the right hand side as K+1. (In the above K is 5)
