
Idea: We want to do ranged query on a set of prefix values.
 
For example, a number like 13 can be written as 1101(in binary). The main Idea is to deconstruct it to query(13) = query(1101) 
1 idea is:			 = query(1000) + query(0100) + query(0001)
another idea is: = query(1000 numbers before 1000) + query(0100 numbers before 1100) + query(0001 numbers before 1101)
another idea is:  instead of query from 13, we query from the minimum power of 2 that is larger than 13, which is 16: 
query(13) -> query(16) -> query(1->8) + query(9 -> 16)
				-> query(1->8) + query(9-> 12) + query(13-> 16)
				 -> query(1->8) + query(9->12) + query(13->13)

These 3 are the ideas that we are going to investigate today, in detail.

## Related Notes  
  
- [[Sparse Table]]  
- [[Fenwick Tree]]  
- [[Segment Tree]]


```

```

