Leetcode
========
Combination Sum: dedupe 'Candidates' first! using 'list(set(.))'

Gas Station: 
1. 1->2->3-*>4, then 1~3 cannot be start. Search from 4 instead.
2. As long as sum of diff[] is positive, such a route/circle must exist.
   Reason: suppose diff[i]>0, then i->i+1. Combine i & i+1 with a single station (gas: diff[i]+gas[i+1]) and the sum of all diffs persist. and so on. 

First Missing Positive: assume sorted array starts from 1!!!
If a[i]=k but a[k-1]=k already, then assign a[i]=0 or -1! In the final step check the first place of 0/-1.
