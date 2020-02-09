Inheritance in interface:

    An interface in Java is a blueprint of a class. It has static constants and abstract methods.
    The interface in Java is a mechanism to achieve abstraction. There can be only abstract methods in the Java interface, not method body. It is used to achieve abstraction and multiple inheritance in Java.
    In other words, you can say that interfaces can have abstract methods and variables. It cannot have a method body.
    Java Interface also represents the IS-A relationship.
    It cannot be instantiated just like the abstract class.
    
  Example:
    
    
            import java.io.*; 
            interface intfA 
            { 
              void m1(); 
            } 

            interface intfB 
            { 
              void m2(); 
            } 

            // class implements both interfaces 
            // and provides implementation to the method. 
            class sample implements intfA, intfB 
            { 
              @Override
              public void m1() 
              { 
                System.out.println("Welcome: inside the method m1"); 
              } 

              @Override
              public void m2() 
              { 
                System.out.println("Welcome: inside the method m2"); 
              } 
            } 

            class GFG 
            { 
              public static void main (String[] args) 
              { 
                sample ob1 = new sample(); 

                // calling the method implemented 
                // within the class. 
                ob1.m1(); 
                ob1.m2(); 
              } 
            } 
 
 output:
 
    Welcome: inside the method m1
    Welcome: inside the method m2
