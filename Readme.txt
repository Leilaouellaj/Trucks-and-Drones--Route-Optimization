We have used 2 sets of coordinates. One was generated randomly from seed 4, the other was manually generated coordinates (With clustered points).  
K can be varied by the condition -I have attached the codes for both. 
forall(i in 2..21) sum(j in 1..LIMIT) Truck_travel_bin(i,j) + sum(j in 1..LIMIT) Drones_travel_bin(i,j)  <= 6
by setting the right hand side as K+1. (In the above K is 5)
