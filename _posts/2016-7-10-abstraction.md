---
layout: post
title:datatypes
---

#Abstraction
<p>Abstraction is a process of hiding the implementation details from the user, only the functionality will be provided to the user. In other words user will have the information on what the object does instead of how it does it.</p>
<h1>Abstract Class</h1>

<p>A class which contains the abstract keyword in its declaration is known as abstract class.

    Abstract classes may or may not contain abstract methods ie., methods with out body ( public void get(); )

    But, if a class have at least one abstract method, then the class must be declared abstract.

    If a class is declared abstract it cannot be instantiated.

    To use an abstract class you have to inherit it from another class, provide implementations to the abstract methods in it.

    If you inherit an abstract class you have to provide implementations to all the abstract methods in it.</p>
    ##Arrays
    <p>An array is a container object that holds a fixed number of values of a single type. The length of an array is established when the array is created. After creation, its length is fixed.</p>
    <p>eclaring a Variable to Refer to an Array

The preceding program declares an array (named anArray) with the following line of code:

// declares an array of integers
int[] anArray;

Like declarations for variables of other types, an array declaration has two components: the array's type and the array's name. An array's type is written as type[], where type is the data type of the contained elements; the brackets are special symbols indicating that this variable holds an array. The size of the array is not part of its type (which is why the brackets are empty). An array's name can be anything you want, provided that it follows the rules and conventions as previously discussed in the naming section. As with variables of other types, the declaration does not actually create an array; it simply tells the compiler that this variable will hold an array of the specified type.</p> 

 
 ##Data types
  int 	A 32-bit (4-byte) integer value
short 	A 16-bit (2-byte) integer value
long 	A 64-bit (8-byte) integer value
byte 	An 8-bit (1-byte) integer value
float 	A 32-bit (4-byte) floating-point value
double 	A 64-bit (8-byte) floating-point value
char 	A 16-bit character using the Unicode encoding scheme
boolean 	A true or false value

  */
package leap.year;

/**
 *
 * @author willie
 */
public class LeapYear {

    /**
     * @param args the command line arguments
     */
    public static void main(String[] args) {
        // TODO code application logic here
        int theYear;
        int y;
        theYear =y;
        if (theYear<100){
            if (theYear>40){ theYear=theYear +1900;
            } else {
                theYear=theYear +2000;
            }
        }
        if(theYear %4==0){
            if(theYear %100 !=0){
                System.out.println("IT IS A LEAP YEAR");
            }else if (theYear% 400==0){
                System.out.println("IT IS A LEAP YEAR");}
            else{
                System.out.println("IT IS NOT A LEAP YEAR");
            }
        }else{
            System.out.println("IT IS NOT A LEAP YEAR");
            }
    }
    
}

  