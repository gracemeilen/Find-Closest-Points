# Data-Structure-and-Algorithms
The Naive algorithm uses comparison plain and simple to find the smallest distance. It compares every set of two points to every other set of two points. 
The DC algorithm recursively breaks down the set of points until it gets down to a set size of 2 then compares the distance between those two points to a globally accessible variable that store the smallest distances found by the algorithm thus far. Storing the points associated with that distance is done in a similar manner. Every time the global distance variable is updated, two global XYPoint variables are updates to contain the points associated with the distance. These variables can be updated one of two ways: in the divide step or the combine step. 




When the DC algorithm was run 100 times on different sets of points, the results were as follows:
Max: 432 milliseconds
Min: 221 milliseconds
Average: 287.86 milliseconds


When the DC algorithm was run 100 times on the same set of points, the results were as follows:
Max: 284 milliseconds 
Min: 23 milliseconds
Average: 35.15 milliseconds 



CROSSOVER ANALYSIS. 
I conducted 2 sets of analysis for this, one for 100000 iterations and one for 10000 iterations. ****NOTE -  The times provides have not been divided the number of iterations for ease of analysis**** 
 The results are as follows:

For Input Size 25 on 100000 iterations:
DC: 473 milliseconds
Naive: 312 milliseconds
When I repeated this input several times, the Naive algorithm consistently beats the DC algorithm. 

The Crossover point lies between input size 25 and 50 for 100000 iterations. 

For Input Size 50 on 100000 iterations:
DC: 1042 milliseconds
Naive: 1254 milliseconds
When I repeated this input several times, the DC algorithm consistently beats the Naive algorithm. 

For Input Size 100 on 100000 iterations:
DC: 2117 milliseconds
Naive: 4807 milliseconds





For Input Size 25 on 10000 iterations:
DC: 172 milliseconds
Naive: 34 milliseconds
The Naive Algorithm Consistently wins at inputs so small.

For Input Size 100 on 10000 iterations:
DC: 504 milliseconds
Naive: 501 milliseconds. 
After running this trial several times, it seems to be a toss up for which one wins. This is the crossover point for 10000 iterations.

For Input Size 200 on 10000 iterations:
DC: 770 milliseconds
Naive: 2016 milliseconds

For Input Size 1000 on 10000 iterations:
DC: 3647 milliseconds
Naive: 49888 milliseconds


