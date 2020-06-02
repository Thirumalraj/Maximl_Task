from collections import defaultdict
import sys
S=input()
distinct_count=len(set(list(S)))
n=len(S)
occur=defaultdict(int)
start=0
minlen= sys.maxsize
distinct_till_here = 0 
for j in range(n):
    occur[S[j]]+=1
    if occur[S[j]]==1:
      distinct_till_here+=1
    if distinct_count==distinct_till_here:
      while occur[S[start]]>1:
        if occur[S[start]]>1:
          occur[S[start]]-=1
        start+=1
      curr_len=j-start+1
      minlen=min(minlen,curr_len)
print(minlen)
