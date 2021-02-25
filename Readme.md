INTRODUCTION
==============================
The aim of this project is to practice the algorithms and techniques that have been seen during the semester. To be more specific, we will perform the simulation of an M/M/1 queueing system. The project is divided into 3 parts. The first part requires us to generate 1000 random variables between 0 and 1, and perform the Kolmogorov and Chi squared tests on the variables to test their uniformity. The second part is to then take that random generated range of numbers, transform them into exponential distribution and then draw the histogram and Q-Q plot to test its exponentiality. Finally, we use the results from part 2, to simulate a service receiving and processing a 1000 packets. Then testing whether those numbers correlate with thee mathematical analysis from the lectures

![alt text](https://github.com/samueliwuno/Network-Simulation-Project/blob/main/NetSim2021-02-24%20210359.jpg?raw=true)

CODE BREAKDOWN
===================================

 Language used is JavaScript. The buttons call appropriate functions
1.  clicking step1 calls random_generate() which generates random numbers, draws histogram and performs uniformity test
2.  Step2 histogram calls make_histogram() which then calls exponential_rand() which generates the random variates and draws the histogram
3.  Step2 QQplot  calls make_qq() which in turn calls exponential_rand() which generates the random variates, and draws the QQplot
4.  Step3 Average Clients calls step3_graph() which then calls single_server_queue() with different values of lamda(λ) and then generates the average packets in system(L) vs Lamda(λ) graph
5.  Step3 Average delay calls step3_graph_delay() which then calls single_server_queue() with different values of lamda(λ) and then generates the average wait times(Wq) vs Lamda(λ) graph
6.  The single_server_queue() method  generates the service times(st),inter-arrival times[irt], wait times[wt], service start[sts]], and service end times[ste]

TO RUN
===================================
extract all files to the same directory
1.	open NET4001_FInal_Project_part2.html with any supported Browser(Tested in Chrome)
2.	Click buttons sequentially to perform all the requirements
3. 	to test a new set of random numbers, click step 1 again
