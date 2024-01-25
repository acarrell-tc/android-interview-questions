Modern Android Interview Questions
==================================
<!-- TOC -->
* [Modern Android Interview Questions](#modern-android-interview-questions)
* [Java ☕️](#java-)
* [Android](#android)
* [Kotlin](#kotlin)
* [Jetpack Compose 🚀](#jetpack-compose-)
* [Testing 🐛](#testing-)
* [Data Structure](#data-structure)
* [Others](#others)
<!-- TOC -->

Java ☕️
=======

*   What is the diff between encapsulation & abstraction (practical example) — [Check here](https://www.javatpoint.com/abstraction-vs-encapsulation-in-java#:~:text=Abstraction%20is%20a%20feature%20of,issue%20at%20the%20design%20level.)
*   HashMaps vs HashTables — [Check here](https://www.geeksforgeeks.org/differences-between-hashmap-and-hashtable-in-java/)
*   When to use array & ArrayList — [Check here](https://www.javatpoint.com/difference-between-array-and-arraylist)
*   What is the volatile keyword — [Check here](https://www.javatpoint.com/volatile-keyword-in-java#:~:text=Volatile%20keyword%20is%20used%20to,with%20primitive%20type%20or%20objects.)
*   What is the transient keyword — [Check here](https://www.javatpoint.com/transient-keyword)
*   What is a diff between a string buffer & string builder — [Check here](https://www.digitalocean.com/community/tutorials/string-vs-stringbuffer-vs-stringbuilder)
*   Why is string immutable — [Check here](https://www.digitalocean.com/community/tutorials/string-vs-stringbuffer-vs-stringbuilder)
*   Explain multithreading. How two threads pass messages internally — [Handler](https://developer.android.com/reference/android/os/Handler#:~:text=A%20Handler%20allows%20you%20to,is%20bound%20to%20a%20Looper%20.)
*   class A -> extends class B, implements interface C. Both have the same method fun add() {}, Which one will be implemented in class A?  
    [Try yourself](https://pl.kotl.in/fRTo80wWr)
*   What is the difference between String test = new String(“X”) & String test = “X”. Explain String constant pool & String literal — [Check here](https://www.javatpoint.com/string-pool-in-java)

Android
=======

*   When I am in my activity onResume() & get a phone call what will be the lifecycle of the fragment inside my activity — [Try yourself](https://pl.kotl.in/fRTo80wWr)
*   Explain context & applicationContext, also a practical example — [Check here](https://www.geeksforgeeks.org/what-is-context-in-android/#:~:text=Both%20the%20Activity%20and%20Application,both%20extend%20the%20Context%20class.)
*   what is the difference between ViewModel and AndroidViewModel — [Check here](https://stackoverflow.com/questions/44148966/androidviewmodel-vs-viewmodel)
*   what is the diff between MVP & MVVM — [Check here](https://blog.mindorks.com/mvc-mvp-mvvm-architecture-in-android)
*   Tell me any method of broadcast receiver except onReceive() — [Check here](https://developer.android.com/reference/android/content/BroadcastReceiver#summary)
*   How Broadcast receiver is used for the network (WIFI) changes — [Check here](https://www.geeksforgeeks.org/broadcast-receiver-in-android-with-example/)
*   Type of services in Android — [Check here](https://www.geeksforgeeks.org/services-in-android-with-example/)
*   Is the Intent service run on background or main thread — [Check here](https://stackoverflow.com/a/15772151/14241355)
*   Explain FCM foreground & background notifications — [Check here](https://firebase.google.com/docs/cloud-messaging/android/receive)
*   Design patterns in Android — [Check here](https://blog.mindorks.com/mastering-design-patterns-in-android-with-kotlin)
*   What do you think about NavHost in navigation? — [Check here](https://developer.android.com/guide/navigation/navigation-getting-started#add-navhost)
*   Explain database management using SQLite, Room & Realm — [Check here](https://medium.com/bitrise/realm-vs-sqlite-which-database-is-better-for-android-apps-c751dc8b150c)
*   What is a foreign key in Room DB? Why do we use it? — [Check here](https://stackoverflow.com/a/56707343/14241355)
*   What is doze mode, and when is it introduced? — [Check here](https://medium.com/mindorks/you-have-to-know-more-about-doze-mode-3d80f016f8ad)
*   what is ADB, can you tell me any commands? — [Cheatsheet](https://devhints.io/adb)
*   what is linting in Android — [Check here](https://blog.mindorks.com/what-is-lint-what-is-it-used-for)
*   What is Rxjava, and how it works? — [Check here](https://blog.mindorks.com/rxjava-for-android-rxandroid)
*   What are SOLID principles? — [Check here](https://www.geeksforgeeks.org/solid-principle-in-programming-understand-with-real-life-examples/)
*   Have you worked with any other hardware systems? (i.e. I have worked with Clover POS system)
*   What is KMP? — [Check here](https://kotlinlang.org/docs/multiplatform.html)

Kotlin
======

*   What are the benefits of Kotlin over Java
*   Explain the use of lateinit & lazy keywords
*   In any class we have a member variable or function, so how can we make a getter setter of that variable?
*   What is MVVM, and how does it work? what is the use of Live data?
*   What is null safety in Kotlin?
*   What is the diff between Var & Val
*   What is Elvis operator?
*   What is Flow API in Kotlin — [Check here](https://developer.android.com/kotlin/flow)
*   Explain coroutines in kotlin
*   What are scoped functions in kotlin
*   How can you declare a singleton class
*   what is the diff between companion obj & object
*   used extension functions? example
*   what is the diff between static & singleton > Singleton has an instance/object while static class is a bunch of static methods.
*   what is constant
*   Explain @JvmStatic @JvmOverloads @JvmField

> You can get most of the Kotlin **answers** here:  
> [https://blog.mindorks.com/kotlin-android-interview-questions](https://blog.mindorks.com/kotlin-android-interview-questions)

Jetpack Compose 🚀
==================

*   What are the benefits of using Jetpack compose?
*   What is a Composable function?
*   What is a declarative approach?
*   What jetpack compose libraries have you used?
*   Explain compose UI basic components

> Jetpack compose blogs with Github examples: [Jetpack Composers](https://medium.com/jetpack-composers)

Testing 🐛
==========

*   In Unit testing, what is @Before & @Beforeclass annotation used for — [Check here](https://www.baeldung.com/junit-before-beforeclass-beforeeach-beforeall)
*   Why should we use a [Mockito](https://blog.mindorks.com/using-mockito-in-android-unit-testing-as-a-pro) lib?
*   Explain [Unit](https://developer.android.com/training/testing/local-tests) & [Instrumentation](https://developer.android.com/training/testing/instrumented-tests) tests

> Espresso Testing Library: [Espresso UI Testing for Intents](https://medium.com/@mansikothari115/espresso-ui-testing-for-intents-in-android-a81660e8e93)

Data Structure
==============

*   The time complexity of Hash Table — **O(1)**
*   Best for getting the last item — **Stack**
*   Time Complexity of Binary Search — **O(log N)**
*   Which is best Sorting Algo — **Quick Sort**
*   Best performance for finding minimum value — **Array**

Others
======

If you have **5+ years** of experience, it’s recommended to prepare for this section.

*   Explain one of your challenging/exciting/recent project
*   VCS — Git — PR review process, CI/CD process
*   Explain deep linking
*   About NDK, c++
*   What other languages do you know apart from Kotlin?
*   Explain the architecture of the communication application, and what data security measures you take while developing.
*   How do you keep up to date yourself with the latest development?
*   Any contribution to the community? Git, StackOverflow
