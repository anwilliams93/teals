
# OOP Skeleton Code

## `ExampleClass.java`
```java
// File ExampleClass.java 
public class ExampleClass 
{
  // instance variables
  private int instanceInt;
  private String instanceString;
  private char instanceChar;
  private boolean instanceBoolean;
  
  // default no-args constructor
  public ExampleClass() 
  {
    instanceInt = 0;
    instanceString = "default";
    instanceChar = '*';
    instanceBoolean = false;
  }
  
  // initialization constructor
  public ExampleClass(int myInt, String myString, 
                      char myChar, boolean myBoolean)
  {
    instanceInt = myInt;
    instanceString = myString;                  
    instanceChar = myChar;
    instanceBoolean = myBoolean;
  }
  
  // getter - make one for each instance variable
  public int getInstanceInt()
  {
    return instanceInt;
  }
  
  // setter - make one for each instance variable
  public void setInstanceInt(int myInt)
  {
    instanceInt = myInt;
  }
  
  // <other getters/setters for the remaining instance variables>
  
  // example method
  public void exampleMethod(String printMe)
  {
    System.out.println(printMe);
  }
}
```
<div class="page"/>

## `ExampleClassRunner.java`
```java
  // File ExampleClassRunner.java
  public class ExampleClassRunner
  {
    // main method - entry point for your program
    public static void main(String[] args)
    {
      // Create an ExampleClass object with the no-args constructor
      ExampleClass exampleObject = new ExampleClass();
      
      // Call a few methods and print some values
      System.out.print("Calling object's instanceInt getter: ");
      System.out.println(exampleObject.getInstanceInt()); 
      
      System.out.println("Calling object's instanceInt setter");
      exampleObject.setInstanceInt(5);

      System.out.print("Calling object's instanceInt getter: ");
      System.out.println(exampleObject.getInstanceInt()); 

      System.out.print("Calling object's exampleMethod: ");
      exampleObject.exampleMethod("Printy print!");
    }
  }
```

## Output
```
Calling object's instanceInt getter: 0
Calling object's instanceInt setter
Calling object's instanceInt getter: 5
Calling object's exampleMethod: Printy print!
```