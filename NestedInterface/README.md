Nested Interface

        An interface i.e. declared within another interface or class is known as nested interface. The nested interfaces are used to group related interfaces so that they can be easy to maintain. The nested interface must be referred by the outer interface or class. It can't be accessed directly.

Syntax:


    interface interface_name{
    ...
    interface nested_interface_name{
    ...
    }
    }
    
  Example

              public class Demo1 {
          public static void main(String[] args){
          C ob = new C();
          ob.method();
        }
        }

          class A{

          protected interface B{
          void method();
        }
        }


         class C implements A.B{
         public void method() {
         System.out.println("Demo: interface nested inside a class");
        }
        }

  
  Output : 
    
    Demo: interface nested inside a class
