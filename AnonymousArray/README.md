    Anonymous Array in Java

An array without name is known as anonymous array in java. As the array do not have any name so it can be used only once. It is passed as an argument of method. Anonymous array is created and initialized in the same line.


    Syntax:
    // anonymous int array 
    new int[] { 1, 2, 3, 4};  

    // anonymous char array 
    new char[] {'x', 'y', 'z'); 

    // anonymous String array
    new String[] {"Geeks", "for", "Geeks"}; 

    // anonymous multidimensional array
    new int[][] { {10, 20}, {30, 40, 50} };

   
  Example:
  
        class Test { 
        public static void main(String[] args) 
        { 
              // anonymous array 
              sum(new int[]{ 1, 2, 3 }); 
        } 
        public static void sum(int[] a) 
        { 
            int total = 0; 

            // using for-each loop 
            for (int i : a)  
                total = total + i; 

            System.out.println("The sum is:" + total); 
        } 
    } 
  
    output:
The sum is 6
