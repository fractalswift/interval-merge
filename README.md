# interval-merge
Simple functions for merging overlapping intervals


Notes:

    Hi! Thanks for reading.
    
    I split this code over several functions for ease of reading and debugging. 
    It is in jupyter notebook format but also uploaded as a .py file as 
    github sometimes has trouble loading notebooks.
    
    This also makes it easier to handle a variety of different cases (see below).
    
    When writing this code I focused on robustness and readability.
  
    Please note: The code treats the (1,4) (4,6) as non-overlapping but you can change this easily, 
    note is in the code on line 40.
    
    Cases handled:
    
      Example case: 
      
      [(1, 3), (5, 12), (4, 10), (20, 25)]
      
      Extra case 1:
    
         There is more than one overlapping pair e.g: 
         [(1, 3), (5, 12), (4, 10), (20, 25), (27, 29), (19, 23)]
    
      Extra case 2:
    
        There are multiple intervals that overlap each other e.g: 
        [(1, 3), (5, 12), (4, 10), (20, 25), (27, 29), (19, 23), (20, 21)]
    
      Extra case 3:
    
         Interval is backwards, e.g (3, 1)
        
      Extra case 4:
    
        Interval has span of 0 e.g (5, 5)
        
      Extra case 5:
        The list contains multiple copies of same interval, eg:
        [(1, 3), (1, 3) ,(5, 12), (4, 10), (20, 25), (27, 29), (19, 23)]
        
        
