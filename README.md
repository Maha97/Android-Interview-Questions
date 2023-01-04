# Android-Interview-Questions
Kotlin 
What is the difference between Lazy and lateinit and which is better regarding memory usage ?
What is the scope function in Kotlin ?
What is enum and sealed classes ?
when to use @JVMField ?
why using data classes rather than normal classes ?
What is the default identifier for kotlin classes ?
What is the differences between Java and Kotlin pros and cons ?
Answer:
Chack this document :https://www.interviewbit.com/kotlin-interview-questions/#when-keyword-in-kotlin


Solid Principles:
Reference : https://codersee.com/solid-principles-with-kotlin-examples/
1 - Single responsibility -- "A class should has only one reason to change "
2 - Open Closed Principle -- "Software entities (classes, modules, functions, etc.) should be open for extension, but closed for modification"
3- Liskov Substitution  -- " classes deriving from the base class should behave in the same manner as the superclass. Most importantly, if we would decide to replace the base class with the derived one, it should not break the existing functionality.
4 - Interface Segregation -- "Many client-specific interfaces are better than one general-purpose interface"
5- Dependency Inversion -- "Depend upon abstractions, [not] concretions"

Differnce between lazy and lateinit
lateinit used with var.      lazy with val 
used with reference avriables only.  used with primitive or reference
- we use lazy when we need to create an object which contains another object so the we want to not initialize the nested val unless we accessed it
- we use lateinit when we need to tell the compiler that we will take care of initializing the variable later

Immutable Variables — Immutable variables are also known as read-only variables

Data Classes In Kotlin :
contains those functions 
equals() - The equals() function returns true if two objects have the identical contents. It operates similarly to "==," although for Float and Double values it works differently.
hashCode() - The hashCode() function returns the object's hashcode value.
copy() - The copy() function is used to duplicate an object, changing only a few of its characteristics while leaving the rest unaltered.
toString() - This function returns a string containing all of the data class's parameters.

How to create Singleton in Kotlin ?
Using object keyword
How to create static variables in kotlin ?
class myClass{
   companion object{
      val x = 5
      fun myStaticMethod(): String{
         return "This method can be called without object"
      }
   }
   
   Inheritance in abstract class in Kotlin 
   Abstract classes are always open. You do not need to explicitly use open keyword to inherit subclasses from them.
}










