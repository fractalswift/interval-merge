# interval-merge
Simple functions for merging overlapping intervals


Notes:
    
    Split into several functions for ease of reading and debugging
    This also makes it easier to handle a variety of different cases (see below)
  
    The code treads (1,4) (4,6) as non-overlapping but you can change this easily, 
    note is in the code
    
    Cases handled:
    
      Example case:
      
      Extra case 1:
    
         There is more than one overlapping pair
    
      Extra case 2:
    
        There are multiple intervals that overlap each other
    
      Extra case 3:
    
         Interval is backwards, e.g (3, 1)
        
    
      Extra case 4:
    
         Interval has span of 0 e.g (5, 5)
        
