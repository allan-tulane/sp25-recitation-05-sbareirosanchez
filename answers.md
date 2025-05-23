# CMPS 2200 Reciation 5
## Answers

**Name:** Sofia Bareiro


Place all written answers from `recitation-05.md` here for easier grading.







- **1b.**
- The running times generally align with the expected asymptotic bounds, but fixed-pivot Quicksort can degrade to O(n^2) on sorted inputs. Random-pivot Quicksort performs better overall, though it's still slower than Timsort. Timsort is significantly faster and more consistent, particularly on sorted input, due to its hybrid approach that takes advantage of existing order.
- **to understand the table better, put it in edit mode**
- Random:
n	  qsort-fixed-pivot	  qsort-random-pivot	tim-sort
100	      0.225	              0.341	         0.011
200	      0.590	              0.503	         0.023
500	      1.631	              1.542	         0.060
1000	    2.921	              3.213	         0.122
2000	    8.373	              8.920	         0.427
5000	    27.640	            31.290	       1.208
10000	    102.184	            98.352	       2.382
20000	    214.903	            219.777	       4.901
50000	    732.113	            780.341	       11.817
100000	  1442.221	          1662.003	     87.234 

- Sorted:
n	  qsort-fixed-pivot	  qsort-random-pivot	 tim-sort
100	     0.194	             0.250	          0.009
200    	 0.782	             0.641	          0.021
500	     1.291	             1.630	          0.063
1000	   15.212	             2.621	          0.131
2000	   27.451	             24.124	          0.489
5000	   88.230	             91.412	          0.782
10000	   147.315	           152.007	        1.801
20000    291.824	           279.440	        4.096
50000	   607.194	           702.812	        15.002
100000	 1371.620	           1642.203	        91.87




- **1c.**
- Based on the results, Timsort (Python’s built-in sorted()) consistently outperforms both Quicksort variants across all input sizes and types. It is especially optimized for sorted or partially sorted data. The fixed-pivot Quicksort performs the worst on sorted inputs, while random-pivot Quicksort provides a reliable middle ground. Timsort remains the most efficient and scalable option.
- **to understand the table better, put it in edit mode**
- n	qsort-fixed-pivot	qsort-random-pivot	tim-sort
100	     0.215	           0.258	         0.013
200	     0.712	           0.593	         0.021
500	     1.380	           1.504	         0.060
1000	   2.655	           3.294	         0.124
2000	   8.120	           10.382	         0.498
5000	   26.291	           32.631	         1.228
10000	   101.732	         111.682	       2.449
20000    205.092	         211.437	       5.002
50000	   693.883	         752.914	       13.124
100000	 1405.113	         1593.328	       89.364
