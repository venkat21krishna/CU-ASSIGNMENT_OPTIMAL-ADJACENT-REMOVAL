# CU-ASSIGNMENT_OPTIMAL-ADJACENT-REMOVAL

#**PLEASE LIKE, SHARE AND SUBSCRIBE THE CHANNEL ****

class Duplicates(object):

   def removeDuplicates(self, S): 
   
      k = []
      
      i = 0
      
      while i < len(S):
      
         if len(k)!=0 and k[-1]==S[i]:
         
            i+=1
            
            k.pop(-1)
            
         else:
         
            k.append(S[i])
            
            i+=1
            
      return len("".join(i for i in k))
      
t=int(input())

for i in range(t):

    s=input()
    
    ob = Duplicates()
    
    print(ob.removeDuplicates(s))
