# Fibonacci Sequence
<h3>Write A Program To Print The Fibonacci Sequence.<br></h3>

<strong><i>Fibonacci Sequence</i></strong>:<p style="font-size:79px"> In mathematics, the Fibonacci numbers, commonly denoted Fn, form a sequence, called the Fibonacci sequence, such that each number is the sum of the two preceding ones, starting from 0 and 1. The sequence starts: 0, 1, 1, 2, 3, 5, 8, 13, 21, 34, 55, 89, 144, ....
<br>The next number is found by adding up the two numbers before it:
<ul>
<li>the 2 is found by adding the two numbers before it (1+1)</li>
<li>the 3 is found by adding the two numbers before it (1+2)</li>
<li>the 5 is (2+3), and so on!</li>
</ul>
</p>


Input:

```Python
Enter number of elements required : 4
```

Output:

```Python
Fibonacci Sequence for 4 elements is : 0, 1, 1, 2
```

class Fibonacci{
    
   // Function to print n Fibonacci series
   public static void fibSequence(int n){
      
       int num1 = 0, num2 = 1;
       int counter = 0;

       // Iterating till counter is N
       while(counter < n){

           // Printing the number
            System.out.print("Fibonacci Sequence of " + n + " elements is : " num1 + " ");
    
            // Swapping
            int num3 = num2 + num1;
            num1 = num2;
            num2 = num3;
            counter += 1; 
       } 
   }
  
    public static void main(String args[]){
   
      Scanner sc = new Scanner(System.in);
      System.out.print(" Enter  number of elements required : ");
      int n = sc.nextInt();
      fibSequence(n); // Function call
    }

}
