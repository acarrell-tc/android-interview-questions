Dependency Injection Interview Questions
========================================

* [What is Dependency Injection (DI) and why do we need it?](#what-is-dependency-injection-di-and-why-do-we-need-it)
* [Can you explain the concept of Inversion of Control (IoC) in relation to DI?](#can-you-explain-the-concept-of-inversion-of-control-ioc-in-relation-to-di)
* [What are the different types of DI?](#what-are-the-different-types-of-di)
* [What is Constructor Injection? Can you give an example using Kotlin?](#what-is-constructor-injection-can-you-give-an-example-using-kotlin)
* [What is Field Injection? Can you provide an example using Kotlin?](#what-is-field-injection-can-you-provide-an-example-using-kotlin)
* [What is Dagger2?](#what-is-dagger2)
* [What is the role of Dagger’s @Inject annotation?](#what-is-the-role-of-daggers-inject-annotation)
* [What is a Dagger Component and what does it do?](#what-is-a-dagger-component-and-what-does-it-do)
* [What is a Dagger Module?](#what-is-a-dagger-module)
* [What is a Subcomponent in Dagger?](#what-is-a-subcomponent-in-dagger)
* [What is Dagger’s @Scope annotation?](#what-is-daggers-scope-annotation)
* [What is Hilt and how is it related to Dagger?](#what-is-hilt-and-how-is-it-related-to-dagger)
* [What is the role of Hilt’s @AndroidEntryPoint annotation?](#what-is-the-role-of-hilts-androidentrypoint-annotation)
* [What is the use of @ViewModelInject in Hilt?](#what-is-the-use-of-viewmodelinject-in-hilt)
* [What are some benefits of using DI in Android development?](#what-are-some-benefits-of-using-di-in-android-development)
* [How can we do DI without using a DI library?](#how-can-we-do-di-without-using-a-di-library)
* [Can you provide an example of how to create a custom @Scope?](#can-you-provide-an-example-of-how-to-create-a-custom-scope)
* [How do you test a class that has dependencies?](#how-do-you-test-a-class-that-has-dependencies)
* [What are potential downsides of DI?](#what-are-potential-downsides-of-di)

### What is Dependency Injection (DI) and why do we need it?

DI is a design pattern that allows an object to receive its dependencies from the outside, rather than creating them
itself. This increases modularity, enhances testability, and improves maintainability by reducing coupling between
modules.

### Can you explain the concept of Inversion of Control (IoC) in relation to DI?

IoC is a design principle in which the control flow of a program is inverted, moving the responsibility of managing
system dependencies from the main program to a framework or container. DI is a form of IoC, where object dependencies
are injected by the system rather than being created by the object.

### What are the different types of DI?

There are three types of DI: Constructor Injection, Method Injection, and Field Injection.

### What is Constructor Injection? Can you give an example using Kotlin?

In constructor injection, the dependencies are provided through a class constructor. Here’s an example:

```kotlin
class MyClass(private val dependency: MyDependency) {
    // ...
}
```

What is Method Injection? Can you provide a Kotlin example?
In method injection, the injector uses a setter method to inject the dependency. Here’s an example:

```kotlin
class MyClass {
    lateinit var dependency: MyDependency

    fun setDependency(dependency: MyDependency) {
        this.dependency = dependency
    }
}
```

### What is Field Injection? Can you provide an example using Kotlin?

In field injection, the injector directly injects the dependencies into the class fields. Here’s an example:

```kotlin
class MyClass {
    @Inject
    lateinit var dependency: MyDependency
}
```

### What is Dagger2?

Dagger2 is a compile-time DI framework for Java, Kotlin, and Android. It generates code to handle object creation and
dependency management, reducing runtime overhead.

### What is the role of Dagger’s @Inject annotation?

The @Inject annotation is used to instruct Dagger that a class or field requires dependencies. Dagger will then generate
the necessary code to provide these dependencies.

### What is a Dagger Component and what does it do?

A Component in Dagger is an interface that serves as a bridge between the modules (providing dependencies) and the
classes that require those dependencies. Dagger generates code for these interfaces.

### What is a Dagger Module?

A Dagger Module is a class annotated with @Module which provides dependencies, i.e., tells Dagger how to construct
objects.

### What is a Subcomponent in Dagger?

A Subcomponent in Dagger is a component that inherits the entire object graph of its parent.

### What is Dagger’s @Scope annotation?

@Scope is used in Dagger to control the lifecycle of an instance created by the Dagger component. Commonly used scopes
are @Singleton, @ActivityScope, @FragmentScope, etc.

### What is Hilt and how is it related to Dagger?

Hilt is a DI library built on top of Dagger to simplify Dagger setup in Android apps. It manages the lifecycle of Dagger
components for you, ensuring they’re properly scoped to match Android’s component lifecycle.

### What is the role of Hilt’s @AndroidEntryPoint annotation?

@AndroidEntryPoint is a Hilt annotation indicating that Hilt should provide some or all of the dependencies for that
class.

### What is the use of @ViewModelInject in Hilt?

The @ViewModelInject annotation allows Hilt to inject dependencies into your ViewModel. It has been deprecated in favour
of @HiltViewModel which is now recommended.

### What are some benefits of using DI in Android development?

DI simplifies code testing by making it easy to swap dependencies with mocks or fakes. It also increases code
reusability and readability, and decreases coupling.

### How can we do DI without using a DI library?

You can do manual DI by creating classes that are responsible for providing dependencies (essentially, factories), and
passing them to the classes that need them. However, this can become complex in large applications, which is why DI
libraries are often used.

### Can you provide an example of how to create a custom @Scope?

In Dagger, you can create a custom scope like this:

```kotlin
@Scope
@Retention(AnnotationRetention.RUNTIME)
annotation class CustomScope
```

### How do you test a class that has dependencies?

DI makes it easier to test classes by replacing real dependencies with mock objects. Here’s an example using Mockito in
a Kotlin test:

```kotlin
class MyTest {
    @Mock
    lateinit var mockDependency: MyDependency
    lateinit var myClass: MyClass

    @BeforeEach
    fun setup() {
        MockitoAnnotations.initMocks(this)
        myClass = MyClass(mockDependency)
    }
}
```

### What are potential downsides of DI?

Some potential downsides include the added complexity of setup, learning curve for DI libraries, and the increased
difficulty of following program flow, especially with compile-time DI libraries like Dagger.

Source: https://medium.com/interviewhackingninja/20-dependency-injection-di-interview-questions-1d8b28529123