algo. for dead lock detection of deadlock
Steps of Algorithm: 
 

    Let Work and Finish be vectors of length m and n respectively. Initialize Work= Available. For i=0, 1, …., n-1, if Requesti = 0, then Finish[i] = true; otherwise, Finish[i]= false.
    Find an index i such that both 
    a) Finish[i] == false 
    b) Requesti <= Work 
    If no such i exists go to step 4.
    Work= Work+ Allocationi 
    Finish[i]= true 
    Go to Step 2.
    If Finish[i]== false for some i, 0<=i<n, then the system is in a deadlocked state. Moreover, if Finish[i]==false the process Pi is deadlock
