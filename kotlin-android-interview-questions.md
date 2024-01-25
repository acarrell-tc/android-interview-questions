Kotlin Android Interview Questions
==================================
<!-- TOC -->
* [Kotlin Android Interview Questions](#kotlin-android-interview-questions)
    * [1\. How does Kotlin work on Android?](#1-how-does-kotlin-work-on-android)
    * [2\. Why should we use Kotlin?](#2-why-should-we-use-kotlin)
    * [3\. What is the difference between the variable declaration with var and val?](#3-what-is-the-difference-between-the-variable-declaration-with-var-and-val)
    * [4\. What is the difference between the variable declaration with val and const?](#4-what-is-the-difference-between-the-variable-declaration-with-val-and-const)
    * [5\. How to ensure null safety in Kotlin?](#5-how-to-ensure-null-safety-in-kotlin)
    * [6\. What is the difference between safe calls(?.) and null check(!!)?](#6-what-is-the-difference-between-safe-calls-and-null-check)
    * [7\. Do we have a ternary operator in Kotlin just like java?](#7-do-we-have-a-ternary-operator-in-kotlin-just-like-java)
    * [8\. What is Elvis operator in Kotlin?](#8-what-is-elvis-operator-in-kotlin)
    * [9\. How to convert a Kotlin source file to a Java source file?](#9-how-to-convert-a-kotlin-source-file-to-a-java-source-file)
    * [10\. What is the use of @JvmStatic, @JvmOverloads, and @JvmFiled in Kotlin?](#10-what-is-the-use-of-jvmstatic-jvmoverloads-and-jvmfiled-in-kotlin)
    * [11\. What is a data class in Kotlin?](#11-what-is-a-data-class-in-kotlin)
    * [12\. Can we use primitive types such as int, double, float in Kotlin?](#12-can-we-use-primitive-types-such-as-int-double-float-in-kotlin)
    * [13\. What is String Interpolation in Kotlin?](#13-what-is-string-interpolation-in-kotlin)
    * [14\. What do you mean by destructuring in Kotlin?](#14-what-do-you-mean-by-destructuring-in-kotlin)
    * [15\. When to use the lateinit keyword in Kotlin?](#15-when-to-use-the-lateinit-keyword-in-kotlin)
    * [16\. How to check if a lateinit variable has been initialized or not?](#16-how-to-check-if-a-lateinit-variable-has-been-initialized-or-not)
    * [17\. What is the difference between lateinit and lazy in Kotlin?](#17-what-is-the-difference-between-lateinit-and-lazy-in-kotlin)
    * [18\. Is there any difference between == operator and === operator?](#18-is-there-any-difference-between--operator-and--operator)
    * [19\. What is the forEach in Kotlin?](#19-what-is-the-foreach-in-kotlin)
    * [20\. What are companion objects in Kotlin?](#20-what-are-companion-objects-in-kotlin)
    * [21\. What is the equivalent of Java static methods in Kotlin?](#21-what-is-the-equivalent-of-java-static-methods-in-kotlin)
    * [22\. What is the difference between FlatMap and Map in Kotlin?](#22-what-is-the-difference-between-flatmap-and-map-in-kotlin)
    * [23\. What is the difference between List and Array types in Kotlin?](#23-what-is-the-difference-between-list-and-array-types-in-kotlin)
    * [24\. Can we use the new keyword to instantiate a class object in Kotlin?](#24-can-we-use-the-new-keyword-to-instantiate-a-class-object-in-kotlin)
    * [25\. What are visibility modifiers in Kotlin?](#25-what-are-visibility-modifiers-in-kotlin)
    * [26\. How to create a Singleton class in Kotlin?](#26-how-to-create-a-singleton-class-in-kotlin)
    * [27\. What are init blocks in Kotlin?](#27-what-are-init-blocks-in-kotlin)
    * [28\. What are the types of constructors in Kotlin?](#28-what-are-the-types-of-constructors-in-kotlin)
    * [29\. Is there any relationship between primary and secondary constructors?](#29-is-there-any-relationship-between-primary-and-secondary-constructors)
    * [30\. What is the default type of argument used in a constructor?](#30-what-is-the-default-type-of-argument-used-in-a-constructor)
    * [31\. What are Coroutines in Kotlin?](#31-what-are-coroutines-in-kotlin)
    * [32\. What is suspend function in Kotlin Coroutines?](#32-what-is-suspend-function-in-kotlin-coroutines)
    * [33\. What is the difference between Launch and Async in Kotlin Coroutines?](#33-what-is-the-difference-between-launch-and-async-in-kotlin-coroutines)
    * [34\. What are scopes in Kotlin Coroutines?](#34-what-are-scopes-in-kotlin-coroutines)
    * [35\. How Exception Handling is done in Kotlin Coroutines?](#35-how-exception-handling-is-done-in-kotlin-coroutines)
    * [36\. How to choose between a switch and when in Kotlin?](#36-how-to-choose-between-a-switch-and-when-in-kotlin)
    * [37\. What is the open keyword in Kotlin used for?](#37-what-is-the-open-keyword-in-kotlin-used-for)
    * [38\. What are lambdas expressions?](#38-what-are-lambdas-expressions)
    * [39\. What are Higher-Order functions in Kotlin?](#39-what-are-higher-order-functions-in-kotlin)
    * [40\. What are extension functions in Kotlin?](#40-what-are-extension-functions-in-kotlin)
    * [41\. What is an infix function in Kotlin?](#41-what-is-an-infix-function-in-kotlin)
    * [42\. What is an inline function in Kotlin?](#42-what-is-an-inline-function-in-kotlin)
    * [43\. What is noinline in Kotlin?](#43-what-is-noinline-in-kotlin)
    * [44\. What are Reified types in Kotlin?](#44-what-are-reified-types-in-kotlin)
    * [45\. What is the operator overloading in Kotlin?](#45-what-is-the-operator-overloading-in-kotlin)
    * [46\. Explain the use-case of let, run, with, also, apply in Kotlin.](#46-explain-the-use-case-of-let-run-with-also-apply-in-kotlin)
    * [47\. What are pair and triple in Kotlin?](#47-what-are-pair-and-triple-in-kotlin)
    * [48\. What are labels in Kotlin?](#48-what-are-labels-in-kotlin)
    * [49\. What are the benefits of using a Sealed Class over Enum?](#49-what-are-the-benefits-of-using-a-sealed-class-over-enum)
    * [50\. What are collections in Kotlin?](#50-what-are-collections-in-kotlin)
<!-- TOC -->
#### 1\. How does Kotlin work on Android?

Just like Java, the Kotlin code is also compiled into the Java bytecode and is executed at runtime by the Java Virtual Machine i.e. JVM. When a Kotlin file named `Main.kt` is compiled then it will eventually turn into a class and then the bytecode of the class will be generated. The name of the bytecode file will be `MainKt.class` and this file will be executed by the JVM.

#### 2\. Why should we use Kotlin?

*   Kotlin is concise
*   Kotlin is null-safe
*   Kotlin is interoperable

[Learn about these features from MindOrks video](https://www.youtube.com/watch?v=kRhivT-jKzY&list=PL6nth5sRD25iv8jZrQWD-5dXgu56ae5m8) .

#### 3\. What is the difference between the variable declaration with var and val?

If you want to declare some mutable(changeable) variable, then you can use `var` . For the immutable variable, use `val` i.e. `val` variables can't be changed once assigned.

#### 4\. What is the difference between the variable declaration with val and const?

Both the variables that are declared with `val` and `const` are immutable in nature. But the value of the `const` variable must be known at the compile-time whereas the value of the `val` variable can be assigned at runtime also.

[Learn more about the difference between const and val from MindOrks blog](https://blog.mindorks.com/what-is-the-difference-between-const-and-val) .

#### 5\. How to ensure null safety in Kotlin?

One of the major advantages of using Kotlin is null safety. In Java, if you access some null variable then you will get a `NullPointerException` . So, the following code in Kotlin will produce a compile-time error:

    var name: String = "MindOrks"
    name = null //error

So, to assign null values to a variable, you need to declare the `name` variable as a nullable string and then during the access of this variable, you need to use a safe call operator i.e. `?.`

    var name: String? = "MindOrks"
    print(name?.length) // ok
    name = null // ok

[Learn more about safe calls(?.) and null check(!!) from MindOrks blog](https://blog.mindorks.com/safecalls-vs-nullchecks-in-kotlin) .

#### 6\. What is the difference between safe calls(?.) and null check(!!)?

Safe call operator i.e. `?.` is used to check if the value of the variable is null or not. If it is null then null will be returned otherwise it will return the desired value.

    var name: String? = "MindOrks"
    println(name?.length) // 8
    name = null
    println(name?.length) // null

If you want to throw NullPointerException when the value of the variable is null, then you can use the null check or `!!` operator.

    var name: String? = "MindOrks"
    println(name?.length) // 8
    name = null
    println(name!!.length) // KotlinNullPointerException

[Learn more about safe calls(?.) and null check(!!) from MindOrks blog](https://blog.mindorks.com/safecalls-vs-nullchecks-in-kotlin) .

#### 7\. Do we have a ternary operator in Kotlin just like java?

No, we don't have a ternary operator in Kotlin but you can use the functionality of ternary operator by using if-else or Elvis operator.

#### 8\. What is Elvis operator in Kotlin?

In Kotlin, you can assign null values to a variable by using the null safety property. To check if a value is having null value then you can use if-else or can use the Elvis operator i.e. `?:` For example:

    var name:String? = "Mindorks"
    val nameLength = name?.length ?: -1
    println(nameLength)

The Elvis operator( `?:` ) used above will return the length of name if the value is not null otherwise if the value is null, then it will return `-1` .

#### 9\. How to convert a Kotlin source file to a Java source file?

Steps to convert your Kotlin source file to Java source file:

1.  Open your Kotlin project in the IntelliJ IDEA / Android Studio.
2.  Then navigate to **Tools > Kotlin > Show Kotlin Bytecode.**
3.  Now click on the **Decompile** button to get your Java code from the bytecode.

[Learn more about the conversion steps from MindOrks blog](https://blog.mindorks.com/how-to-convert-a-kotlin-source-file-to-a-java-source-file) .

#### 10\. What is the use of @JvmStatic, @JvmOverloads, and @JvmFiled in Kotlin?

*   **@JvmStatic:** This annotation is used to tell the compiler that the method is a static method and can be used in Java code.
*   **@JvmOverloads:** To use the default values passed as an argument in Kotlin code from the Java code, we need to use the `@JvmOverloads` annotation.
*   **@JvmField:** To access the fields of a Kotlin class from Java code without using any getters and setters, we need to use the `@JvmField` in the Kotlin code.

[Learn more about @JvmStatic, @JvmOverloads, and @JvmField in Kotlin from MindOrks blog](https://amitshekhar.me/blog/jvmstatic-annotation-in-kotlin) .

#### 11\. What is a data class in Kotlin?

Data classes are those classes which are made just to store some data. In Kotlin, it is marked as data. The following is an example of the same:

    data class Developer(val name: String, val age: Int)

When we mark a class as a _data_ class, you don’t have to implement or create the following functions like we do in Java: `hashCode()` , `equals()` , `toString()` , `copy()` . The compiler automatically creates these internally, so it also leads to clean code. Although, there are few other requirements that data classes need to fulfill.

[Learn more about data class from MindOrks blog](https://blog.mindorks.com/learn-kotlin-data-class) .

#### 12\. Can we use primitive types such as int, double, float in Kotlin?

In Kotlin, we can't use primitive types directly. We can use classes like Int, Double, etc. as an object wrapper for primitives. But the compiled bytecode has these primitive types.

#### 13\. What is String Interpolation in Kotlin?

If you want to use some variable or perform some operation inside a string then String Interpolation can be used. You can use the `$` sign to use some variable in the string or can perform some operation in between `{}` sign.

    var name = "MindOrks"
    print("Hello! I am learning from $name")

#### 14\. What do you mean by destructuring in Kotlin?

**Destructuring** is a convenient way of extracting multiple values from data stored in(possibly nested) objects and Arrays. It can be used in locations that receive data (such as the left-hand side of an assignment). Sometimes it is convenient to destructure an object into a number of variables, for example:

    val (name, age) = developer

Now, we can use name and age independently like below:

    println(name)
    println(age)

[Learn more about Kotlin Destructuring from MindOrks blog](https://blog.mindorks.com/learn-kotlin-destructuring-declarations) .

#### 15\. When to use the lateinit keyword in Kotlin?

`lateinit` is late initialization.

Normally, properties declared as having a non-null type must be initialized in the constructor. However, fairly often this is not convenient.

For example, properties can be initialized through dependency injection, or in the setup method of a unit test. In this case, you cannot supply a non-null initializer in the constructor, but you still want to avoid null checks when referencing the property inside the body of a class. To handle this case, you can mark the property with the lateinit modifier.

[Learn more about lateinit from MindOrks blog](https://amitshekhar.me/blog/lateinit-vs-lazy-in-kotlin) .

#### 16\. How to check if a lateinit variable has been initialized or not?

You can check if the lateinit variable has been initialized or not before using it with the help of `isInitialized` method. This method will return true if the lateinit property has been initialized otherwise it will return false. For example:

    class Person {
     lateinit var name: String
     fun initializeName() {
     println(this::name.isInitialized)
     name = "MindOrks" // initializing name
     println(this::name.isInitialized)
     }
    }
    fun main(args: Array<String>) {
     Person().initializeName()
    }

[Learn more about it from MindOrks blog](https://blog.mindorks.com/how-to-check-if-a-lateinit-variable-has-been-initialized) .

#### 17\. What is the difference between lateinit and lazy in Kotlin?

*   lazy can only be used for val properties, whereas lateinit can only be applied to var because it can’t be compiled to a final field, thus no immutability can be guaranteed.
*   If you want your property to be initialized from outside in a way probably unknown beforehand, use lateinit.

[Learn more about the difference between lateinit and lazy from MindOrks blog](https://amitshekhar.me/blog/lateinit-vs-lazy-in-kotlin) .

#### 18\. Is there any difference between == operator and === operator?

Yes. The `==` operator is used to compare the values stored in variables and the `===` operator is used to check if the reference of the variables are equal or not. But in the case of primitive types, the `===` operator also checks for the value and not reference.

    // primitive example
    val int1 = 10 
    val int2 = 10
    println(int1 == int2) // true
    println(int1 === int2) // true
    // wrapper example
    val num1 = Integer(10)
    val num2 = Integer(10)
    println(num1 == num2) // true
    println(num1 === num2) //false

#### 19\. What is the forEach in Kotlin?

In Kotlin, to use the functionality of a for-each loop just like in Java, we use a `forEach` function. The following is an example of the same:

    var listOfMindOrks = listOf("mindorks.com", "blog.mindorks.com", "afteracademy.com")
    listOfMindOrks.forEach {
     Log.d(TAG,it)
    }

#### 20\. What are companion objects in Kotlin?

In Kotlin, if you want to write a function or any member of the class that can be called without having the instance of the class then you can write the same as a member of a companion object inside the class.

To create a **companion** object, you need to add the `companion` keyword in front of the object declaration.

The following is an example of a companion object in Kotlin:

    class ToBeCalled {
     companion object Test {
     fun callMe() = println("You are calling me :)")
     }
    }
    fun main(args: Array<String>) {
     ToBeCalled.callMe()
    }

[Learn more about companion object from MindOrks blog](https://blog.mindorks.com/companion-object-in-kotlin) .

#### 21\. What is the equivalent of Java static methods in Kotlin?

To achieve the functionality similar to Java static methods in Kotlin, we can use:

*   companion object
*   package-level function
*   object

[Read more about this from MindOrks blog](https://blog.mindorks.com/what-is-the-equivalent-of-java-static-methods-in-kotlin) .

#### 22\. What is the difference between FlatMap and Map in Kotlin?

*   FlatMap is used to combine all the items of lists into one list.
*   Map is used to transform a list based on certain conditions.

[Read more about FlatMap and Map in Kotlin from MindOrks blog](https://blog.mindorks.com/flatmap-vs-map-in-kotlin) .

#### 23\. What is the difference between List and Array types in Kotlin?

If you have a list of data that is having a fixed size, then you can use an Array. But if the size of the list can vary, then we have to use a mutable list.

[Learn more about the difference between List and Array from MindOrks blog](https://blog.mindorks.com/difference-between-list-and-array-types-in-kotlin) .

#### 24\. Can we use the new keyword to instantiate a class object in Kotlin?

No, in Kotlin we don't have to use the `new` keyword to instantiate a class object. To instantiate a class object, simply we use:

    var varName = ClassName()

#### 25\. What are visibility modifiers in Kotlin?

A visibility modifier or access specifier or access modifier is a concept that is used to define the scope of something in a programming language. In Kotlin, we have four visibility modifiers:

*   **private:** visible inside that particular class or file containing the declaration.
*   **protected:** visible inside that particular class or file and also in the subclass of that particular class where it is declared.
*   **internal:** visible everywhere in that particular module.
*   **public:** visible to everyone.

Note: By default, the visibility modifier in Kotlin is **public** .

[Learn more about visibility modifiers in Kotlin from MindOrks blog](https://blog.mindorks.com/learn-kotlin-visibility-modifiers-private-protected-internal-public) .

#### 26\. How to create a Singleton class in Kotlin?

A singleton class is a class that is defined in such a way that only one instance of the class can be created and is used where we need only one instance of the class like in logging, database connections, etc.

To create a Singleton class in Kotlin, you need to use the object keyword.

    object AnySingletonClassName

> Note: You can't use constructor in object, but you can use init.

[Learn more about Singleton class from MindOrks blog](https://blog.mindorks.com/how-to-create-a-singleton-class-in-kotlin) .

#### 27\. What are init blocks in Kotlin?

`init` blocks are initializer blocks that are executed just after the execution of the primary constructor. A class file can have one or more init blocks that will be executed in series. If you want to perform some operation in the primary constructor, then it is not possible in Kotlin, for that, you need to use the `init` block.

[Learn more about init blocks from MindOrks blog](https://blog.mindorks.com/understanding-init-block-in-kotlin) .

#### 28\. What are the types of constructors in Kotlin?

*   **Primary constructor:** These constructors are defined in the class header and you can't perform some operation in it, unlike Java's constructor.
*   **Secondary constructor:** These constructors are declared inside the class body by using the constructor keyword. You must call the primary constructor from the secondary constructor explicitly. Also, the property of the class can’t be declared inside the secondary constructor. There can be more than one secondary constructors in Kotlin.

[Learn more about Primary and Secondary constructors from MindOrks blog](https://blog.mindorks.com/primary-and-secondary-constructors-in-kotlin) .

#### 29\. Is there any relationship between primary and secondary constructors?

Yes, when using a secondary constructor, you need to call the primary constructor explicitly.

#### 30\. What is the default type of argument used in a constructor?

By default, the type of arguments of a constructor in val. But you can change it to var explicitly.

#### 31\. What are Coroutines in Kotlin?

A framework to manage concurrency in a more performant and simple way with its lightweight thread which is written on top of the actual threading framework to get the most out of it by taking the advantage of cooperative nature of functions.

**This is an important interview question** .

[Learn more about Kotlin Coroutines with examples from MindOrks blog](https://amitshekhar.me/blog/kotlin-coroutines) .

#### 32\. What is suspend function in Kotlin Coroutines?

Suspend function is the building block of the Coroutines in Kotlin. Suspend function is a function that could be started, paused, and resume. To use a suspend function, we need to use the suspend keyword in our normal function definition.

[Learn more about the suspend function from MindOrks blog](https://amitshekhar.me/blog/suspend-function-in-kotlin-coroutines) .

#### 33\. What is the difference between Launch and Async in Kotlin Coroutines?

The difference is that the `launch{}` does not return anything and the `async{}` returns an instance of `Deferred<T>` , which has an `await()` function that returns the result of the coroutine like we have future in Java in which we do `future.get()` to the get the result.

In other words:

*   launch: fire and forget
*   async: perform a task and return a result

[Learn more about Launch vs Async from MindOrks video](https://www.youtube.com/watch?v=nC30UiDv8Xc) .

#### 34\. What are scopes in Kotlin Coroutines?

[Learn from MindOrks blog](https://amitshekhar.me/blog/kotlin-coroutines) .

#### 35\. How Exception Handling is done in Kotlin Coroutines?

[Learn from MindOrks blog](https://blog.mindorks.com/exception-handling-in-kotlin-coroutines) .

#### 36\. How to choose between a switch and when in Kotlin?

Whenever we want to handle many if-else conditions, then we generally use switch-case statements. But Kotlin provides a more concise option i.e. in Kotlin, we can use when in place of the switch. And, when can be used as:

*   expression
*   arbitrary condition expression
*   without argument
*   with two or more choices

For example:

    when(number) {
     1 -> println("One")
     2, 3 -> println("Two or Three")
     4 -> println("Four")
     else -> println("Number is not between 1 and 4")
    }

[Learn more about when from MindOrks blog](https://blog.mindorks.com/replace-switch-with-when-in-kotlin) .

#### 37\. What is the open keyword in Kotlin used for?

By default, the classes and functions are final in Kotlin. So, you can't inherit the class or override the functions. To do so, you need to use the open keyword before the class and function. For example:

[Learn more about open keyword from MindOrks blog](https://blog.mindorks.com/understanding-open-keyword-in-kotlin) .

#### 38\. What are lambdas expressions?

Lambdas expressions are anonymous functions that can be treated as values i.e. we can pass the lambdas expressions as arguments to a function return them, or do any other thing we could do with a normal object. For example:

    val add : (Int, Int) -> Int = { a, b -> a + b }
    val result = add(9, 10)

[Learn more about Lambdas from MindOrks blog](https://amitshekhar.me/blog/higher-order-functions-and-lambdas-in-kotlin) .

#### 39\. What are Higher-Order functions in Kotlin?

A higher-order function is a function that takes functions as parameters or returns a function. For example, A function can take functions as parameters.

    fun passMeFunction(abc: () -> Unit) {
     // I can take function
     // do something here
     // execute the function
     abc()
    }

For example, A function can return another function.

    fun add(a: Int, b: Int): Int {
     return a + b
    }

And, we have a function **returnMeAddFunction** which takes zero parameters and returns a function of the type **((Int, Int) -> Int)** .

    fun returnMeAddFunction(): ((Int, Int) -> Int) {
     // can do something and return function as well
     // returning function
     return ::add
    }

And to call the above function, we can do:

    val add = returnMeAddFunction()
    val result = add(2, 2)

[Learn more about Higher-Order functions from MindOrks blog](https://amitshekhar.me/blog/higher-order-functions-and-lambdas-in-kotlin) .

#### 40\. What are extension functions in Kotlin?

Extension functions are like extensive properties attached to any class in Kotlin. By using extension functions, you can add some methods or functionalities to an existing class even without inheriting the class. For example: Let's say, we have views where we need to play with the visibility of the views. So, we can create an extension function for views like,

    fun View.show() {
     this.visibility = View.VISIBLE
    }
    
    fun View.hide() {
     this.visibility = View.GONE
    }

and to use it we use, like,

    toolbar.hide()

[Learn more about extension functions from MindOrks blog](https://blog.mindorks.com/extension-functions-vs-static-utility-class) .

#### 41\. What is an infix function in Kotlin?

An infix function is used to call the function without using any bracket or parenthesis. You need to use the infix keyword to use the infix function.

    class Operations {
     var x = 10; 
     infix fun minus(num: Int) {
     	this.x = this.x - num
     } 
    }
    fun main() {
     val opr = Operations()
     opr minus 8
     print(opr.x)
    }

#### 42\. What is an inline function in Kotlin?

Inline function instruct compiler to insert complete body of the function wherever that function got used in the code. To use an Inline function, all you need to do is just add an inline keyword at the beginning of the function declaration.

[Learn more about Inline functions from MindOrks blog](https://amitshekhar.me/blog/inline-function-in-kotlin) .

#### 43\. What is noinline in Kotlin?

While using an inline function and want to pass some lambda function and not all lambda function as inline, then you can explicitly tell the compiler which lambda it shouldn't inline.

    inline fun doSomethingElse(abc: () -> Unit, noinline xyz: () -> Unit) {
     abc()
     xyz()
    }

[Learn more about noinline functions from MindOrks blog](https://amitshekhar.me/blog/inline-function-in-kotlin) .

#### 44\. What are Reified types in Kotlin?

When you are using the concept of Generics to pass some class as a parameter to some function and you need to access the type of that class, then you need to use the reified keyword in Kotlin.

For example:

    inline fun <reified T> genericsExample(value: T) {
     println(value)
     println("Type of T: ${T::class.java}")
    }
    fun main() {
     genericsExample<String>("Learning Generics!")
     genericsExample<Int>(100)
    }

[Learn more about Reified keyword from MindOrks blog](https://blog.mindorks.com/what-are-reified-types-in-kotlin) .

#### 45\. What is the operator overloading in Kotlin?

In Kotlin, we can use the same operator to perform various tasks and this is known as operator overloading. To do so, we need to provide a member function or an extension function with a fixed name and operator keyword before the function name because normally also, when we are using some operator then under the hood some function gets called. For example, if you are writing `num1+num2` , then it gets converted to `num1.plus(num2)` .

For example:

    fun main() {
     val bluePen = Pen(inkColor = "Blue")
     bluePen.showInkColor()
    
     val blackPen = Pen(inkColor = "Black")
     blackPen.showInkColor()
    
     val blueBlackPen = bluePen + blackPen
     blueBlackPen.showInkColor()
    }
    
     operator fun Pen.plus(otherPen: Pen):Pen{
     val ink = "$inkColor, ${otherPen.inkColor}"
     return Pen(inkColor = ink)
     }
    
     data class Pen(val inkColor:String){
     fun showInkColor(){ println(inkColor)}
     }

[Learn more about operator overloading from MindOrks blog](https://blog.mindorks.com/operator-overloading-in-kotlin) .

#### 46\. Explain the use-case of let, run, with, also, apply in Kotlin.

[Learn from MindOrks blog](https://blog.mindorks.com/using-scoped-functions-in-kotlin-let-run-with-also-apply) .

#### 47\. What are pair and triple in Kotlin?

Pair and Triples are used to return two and three values respectively from a function and the returned values can be of the same data type or different.

    val pair = Pair("My Age: ", 25)
    print(pair.first + pair.second)

[Learn more about Pairs and Triples from MindOrks blog](https://blog.mindorks.com/pair-and-triple-in-kotlin) .

#### 48\. What are labels in Kotlin?

Any expression written in Kotlin is called a label. For example, if we are having a _for-loop_ in our Kotlin code then we can name that _for-loop_ expression as a label and will use the label name for the _for-loop_ .

We can create a label by using an identifier followed by the `@` sign. For example, `name@` , `loop@` , `xyz@` , etc. The following is an example of a label:

    loop@ for (i in 1..10) {
     // some code goes here
    }

The name of the above for-loop is `loop` .

[Learn more about labels in Kotlin from MindOrks blog](https://blog.mindorks.com/learn-kotlin-returns-jumps-labels) .

#### 49\. What are the benefits of using a Sealed Class over Enum?

Sealed classes give us the flexibility of having **different** **types of subclasses and also containing the state** . The important point to be noted here is the subclasses that are extending the Sealed classes should be either nested classes of the Sealed class or should be declared in the same file as that of the Sealed class.

[Learn more about Sealed classes from MindOrks blog](https://blog.mindorks.com/learn-kotlin-sealed-classes) .

#### 50\. What are collections in Kotlin?

[Learn from MindOrks video](https://www.youtube.com/watch?v=XeRt2ZZ-jkA) .

Prepare these 50 questions for your interview and also go through the given link in each question to have a better knowledge of the topic.

Also, you can find the Android Interview Questions **[here](https://github.com/MindorksOpenSource/android-interview-questions)** .

Share this blog with other developers who are going to give some Android interview.

**All the best for your interview!**

Team MindOrks!

**Also, Let’s connect on** **[Twitter](https://twitter.com/hiii_sumit) ,** **[Linkedin](https://www.linkedin.com/in/mishra3452/) ,** **[Github](https://github.com/mishra3452) , and** **[Facebook](https://www.facebook.com/mishra3452)**
