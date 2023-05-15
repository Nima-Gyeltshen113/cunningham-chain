# cunningham-chain
Find it!
# Python3 program for cunningham chain
 
# Function to print Cunningham chain
# of the first kind
def print_C(p0):
     
    i = 0;
     
    # Iterate till all elements
    # are printed
    while(True):
        flag = 1;
        x = pow(2, i);
        p1 = x * p0 + (x - 1);
         
        # check prime or not
        for k in range(2, p1):
            if (p1 % k == 0):
                flag = 0;
                break;
         
        if (flag == 0):
            break;
         
        print(p1, end = " ");
        i += 1;
 
# Driver Code
p0 = 2;
print_C(p0);
 
# This code is contributed by mits
