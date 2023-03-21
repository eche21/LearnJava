To run HelloWorld.java on the terminal, navigate to the directory containing the java file
and then type  

1. javac HelloWorld.java

2. java -cp . HelloWorld

The first line compiles the source code into executable byte code. The second line executes it, 
first adding the current directory to the class path (just in case).

________________________________________________________________________
A closer look at the Helloworld.java file
________________________________________________________________________

 multiline comment-this type of comment must begin with /* and end with */. 

The next line of code in the program is shown here:

public class HelloWorld {

This line uses the keyword class to declare that a new class is being defined. Example
is an identifier that is the name of the class. The entire class definition, including all of its 
members, will be between the opening curly brace ({) and the closing curly brace (}).


The next line of code is shown here:

public static void main(String args[ ]) {

This line begins the main( ) method. This is the line 
at which the program will begin executing. 


The public keyword is an access modifier, which allows the programmer to control the 
visibility of class members. When a class member is preceded by public, then that member 
may be accessed by code outside the class in which it is declared. (The opposite of public is 
private, which prevents a member from being used by code defined outside of its class.) In 
this case, main( ) must be declared as public, since it must be called by code outside of its 
class when the program is started. The keyword static allows main( ) to be called without 
having to instantiate a particular instance of the class. This is necessary since main( ) is 
called by the Java Virtual Machine before any objects are made. The keyword void simply 
tells the compiler that main( ) does not return a value. 
String args[ ] declares a parameter named args, which is an array of instances of the class 
String. (Arrays are collections of similar objects.) Objects of type String store character 
strings. In this case, args receives any command-line arguments present when the program 
is executed.
The last character on the line is the {. This signals the start of main( )’s body.

The next line in the program is the single-line comment, shown here:

// TODO Auto-generated method stub

This is the second type of comment supported by Java. A single-line comment begins with a // 
and ends at the end of the line.

The next line of code is shown here. Notice that it occurs inside main( ).

System.out.println("Hello World!");

This line outputs the string "Hello World!" followed by a new line on the 
screen. Output is actually accomplished by the built-in println( ) method. In this case, println( )
displays the string which is passed to it. The line begins with System.out.  System is a predefined class that provides access to the system, 
and out is the output stream that is connected to the console.