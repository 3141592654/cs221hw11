# cs221hw11
To run, use make.
I used mostly the same parameters Eitan used; num_iter=9,000,000; pop_size=1000; mut_rate=0.3; nthreads=4 (because my laptop has not quite so many cores as Eitan's desktop). With no parallelism (I.E. the code in the hw10 solution with num_iter = 9 million instead of 2 million), it takes 57.7 seconds. The parallelized version takes 26.5 seconds. My GA does not beat the provided shortest.tsv. The shortest.tsv in this submission is the result of an nthreads=3 execution which lasted 26.181 seconds.

Threads						1			2			4			8 (more threads than I have cores on my laptop)
1-deme parallelism (extracredit)	57.5s7590		42.2s5964		42.0s7170		51.4s6740
n-deme parallelism 				62.5s7023		30.4s6386		26.5s/5876	29.1s5640