**************************** Java Test ****************************************

1. I come up with Quick sort and Bucket sort at the same time but finally I
   chose Quick sort. I've written the details of my Quick sort at the top of
   my Java program. Here I want to talk about my analysis about Bucket sort.
   
   - Use TreeMap as buckets with year, month or day as keys.
   - The map is sorted according to the natural ordering of its keys.
   - Each year bucket contains month buckets and each month bucket contains day
     buckets.
   - Dynamically create and add new bucket in the existing bucket list when needed.
   - Final result should look like this:
   		bucket(1969) -> bucket(1971) -> ...
             |              |
   		     |           /      \
   		    b(6)	   b(2)    b(11)
   		    			|        |
   		    		   / \       |
   		    	   b(15) b(16) b(11)
   - Time complexity is O(n + k). n is number of records and k is total number
     buckets except leaves.
   - Space complexity is O(n + k).
   - The reason why I chose Quick sort is
   		- Easy to achieve: merge string together and sort.
   		- Less space consume
   		- We don't know the range of each level so we can't make sure whether it's
   		  quicker or not.
   		  
   		  
******************************* Vertica Web Test A ****************************
                             
1. Page Layout
	-----------------------------------------
	|	Header								|
	|										|
	-----------------------------------------
	|										|
	|				------------			|
	|				|	DIV	   |			|
	|  DIV Container|floatPanel|		    |
	|				------------			|
	|										|
	-----------------------------------------
	|										|
	|	Footer								|
	-----------------------------------------
	
2. Problems not solved
	- When you first drag the panel which is centered, you need to press down and
	  move mouse upwards until the panel shows up in top left corner of the gray area.
	- When you first drag the panel at lower right corner, you can't drag it to
	  the bottom of the gray area.