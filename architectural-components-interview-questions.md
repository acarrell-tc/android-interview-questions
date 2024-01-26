1. What are Android Architecture Components? Android Architecture
   Answer: Components are a collection of libraries that help you design robust, testable, and maintainable apps. They
   provide a clear and idiomatic way to consume REST APIs. These components include Room, ViewModel, LiveData, and
   others.

2. What is LiveData?
   Answer: LiveData is an observable data holder class that is lifecycle-aware. This means it respects the lifecycle of
   other app components, such as activities, fragments, or services, and only updates app component observers that are
   in an active lifecycle state.

3. What is ViewModel?
   Answer: The ViewModel class is designed to store and manage UI-related data in a lifecycle-conscious way. The
   ViewModel class allows data to survive configuration changes such as screen rotations.

4. What is Room?
   Answer: Room is a persistence library that provides an abstraction layer over SQLite. It allows for more robust
   database access while harnessing the full power of SQLite.

5. How does LiveData work with ViewModel?
   Answer: LiveData can be used in conjunction with ViewModel to update the UI automatically when the data changes.
   ViewModel holds the LiveData objects, and the UI components observe these objects.

6. What are the benefits of using Android Architecture Components?
   Answer: Android Architecture Components can help to construct a robust app architecture, simplify the handling of
   data changes, and ensure that the UI matches the current state of data.

7. What is the purpose of the onCleared() method in ViewModel?
   Answer: The onCleared() method in ViewModel is called when the ViewModel is no longer used and will be destroyed.
   This method is useful to clean up any resources that the ViewModel might be using.

8. What is the difference between LiveData and MutableLiveData?
   Answer: LiveData is an observable data holder class, while MutableLiveData is a LiveData class that exposes the
   setValue(T) and postValue(T) methods publicly. You can use MutableLiveData when you need to change the stored data.

9. What is the advantage of using Room over raw SQLite?
   Answer: Room provides an abstraction layer over SQLite, making it easier and more intuitive to work with databases in
   Android. It includes compile-time checks of SQL queries, reducing the likelihood of runtime SQL errors.

10. What is the role of the Repository in Android Architecture Components?
    Answer: The Repository is a design pattern that mediates between different data sources, such as persistent models,
    web services, and caches. In the context of Android Architecture Components, a Repository manages query threads and
    allows you to use multiple backends.

11. What is Data Binding and how is it useful in Android Architecture Components?
    Answer: Data Binding is a support library that allows you to bind UI components in your layouts to data sources in
    your app using a declarative format rather than programmatically. This reduces boilerplate code and prevents common
    programming errors.

12. What is the lifecycle of a ViewModel?
    Answer: The lifecycle of a ViewModel extends from when you first request a ViewModel until the associated UI
    controller (activity or fragment) is finished completely and is in the destroyed state.

13. What is the difference between setValue() and postValue() in LiveData?
    Answer: setValue(T) method must be called from the main thread. If the code is invoked from a worker thread, you can
    use postValue(T) method instead which posts a task to a main thread to set the given value.

14. How does Room handle object relationships?
    Answer: Room allows you to define Foreign Key relationships between your entities. This ensures integrity at the
    database level by declaring relationships between tables.

15. What is a TypeConverter in Room?
    Answer: Room provides functionality to convert between primitive and boxed types but doesn’t allow for object
    references between entities. This is where TypeConverter comes in. It allows you to convert custom classes to known
    types that Room can persist.

16. What is the role of LiveData in MVVM architecture?
    Answer: In MVVM architecture, LiveData allows data changes in the Model layer to be observed in the ViewModel and
    then automatically reflected in the View layer.

17. What is the difference between ViewModel and AndroidViewModel?
    Answer: AndroidViewModel is a subclass of ViewModel that includes an Application reference. This is useful if, for
    example, you need a context to access SharedPreferences or other Android components.

18. How does Room support LiveData?
    Answer: Room provides built-in support for LiveData. Your DAO methods can return a LiveData object, and Room
    generates all necessary code to update the LiveData object when the database is updated.

19. What is a LiveData Transformations?
    Answer: Transformations are a set of utility methods that can be used to manipulate LiveData objects. For example,
    Transformations.map() applies a function to the output of LiveData and propagates the result downstream.

20. What is the benefit of using a Repository in Android Architecture Components?
    Answer: A Repository class abstracts access to multiple data sources. It handles data operations and allows you to
    use multiple backends such as network, cache, and database. This provides a clean API to the rest of the app and
    helps to achieve separation of concerns.

21. What is the role of Entity in Room?
    Answer: An Entity represents a table within the database. Room creates a table for each class that has @Entity
    annotations, the fields in the class correspond to columns in the table.

22. What is a DAO in Room?
    Answer: DAO stands for Data Access Object. It’s an interface that defines the methods for accessing the database. In
    Room, you annotate a DAO interface or abstract class with @Dao.

23. What is a Database class in Room?
    Answer: The Database class is a holder class that uses annotations to define the list of entities and database
    version. This class content defines the list of tables and version within the database.

24. What is the difference between allowMainThreadQueries() and fallbackToDestructiveMigration() in Room?
    Answer: allowMainThreadQueries() allows Room to execute database operations on the main thread, which is not
    recommended because it can lock the UI. fallbackToDestructiveMigration() allows Room to recreate database tables if
    their schemas have changed.

25. What is the role of Paging Library in Android Architecture Components?
    Answer: The Paging Library helps you load and display small chunks of data at a time. It is useful for when you’re
    working with large data sets that can affect the performance of your app.

26. What is WorkManager in Android Architecture Components?
    Answer: WorkManager is a library used for background work that defers tasks or runs them synchronously. It respects
    the lifecycle and state of your app and has a flexible retry policy.

27. What is DiffUtil in the context of Android Architecture Components?
    Answer: DiffUtil is a utility class that calculates the difference between two lists and outputs a list of update
    operations that converts the first list into the second one.

28. What is LiveData ReActiveStreams?
    Answer: LiveData ReActiveStreams is a library that provides transformations for LiveData that make it easier to
    integrate it with ReactiveStreams, such as RxJava.

29. What is the @Insert annotation in Room?
    Answer: The @Insert annotation is used in Room to mark a method as an insert method. The implementation of the
    method will insert its parameters into the database.

30. What is the @Query annotation in Room?
    Answer: The @Query annotation allows you to write SQL statements and expose them as DAO methods. Room verifies SQL
    queries at compile-time.

31. What is the @Delete annotation in Room?
    Answer: The @Delete annotation is used to mark a method in a DAO class as a delete method. The implementation of the
    method will delete its parameters from the database.

32. What is the @Update annotation in Room?
    Answer: The @Update annotation is used to mark a method in a DAO class as an update method. The implementation of
    the method will update its parameters in the database.

33. What is a ConflictStrategy in Room?
    Answer: ConflictStrategy defines a strategy to resolve conflicts at runtime when inserting or updating data in the
    database.

34. What is a Composite Primary Key in Room?
    Answer: A Composite Primary Key allows you to specify two or more fields as the primary key in Room. This is done
    using the @Entity annotation and specifying the field names in the primaryKeys attribute.

35. What is PagedList in the context of Android Architecture Components?
    Answer: PagedList is a component of the Paging Library. It is a List that loads its data in chunks (pages) from a
    DataSource. It can be observed for changes and accessed in a random-access fashion.

36. What is ViewModelProvider in Android Architecture Components?
    Answer: ViewModelProvider is a utility class that provides ViewModels for a scope. It creates new ViewModels and
    retains them in a store to survive configuration changes.

37. What is ViewModelScope in Android Architecture Components?
    Answer: ViewModelScope is a scope tied to the lifecycle of a ViewModel. It is used to launch coroutines that will be
    cancelled when the ViewModel is cleared.

38. What is LiveDataScope in Android Architecture Components?
    Answer: LiveDataScope is a scope for a block of code that is producing a LiveData value. It is used with the
    liveData builder function.

39. What is the @Transaction annotation in Room?
    Answer: The @Transaction annotation is used in Room to mark a method as a transaction method. The implementation of
    the method will be run in a single transaction.

40. What is Flow in the context of Android Architecture Components?
    Answer: Flow is a type in Kotlin’s coroutines library that is used for handling streams of data asynchronously. Room
    provides APIs to return query results as a Flow.

41. What is DataSource.Factory in the context of Android Architecture Components?
    Answer: DataSource.Factory is a factory class for data sources. It is used with the Paging Library to create a
    DataSource for paging data from a database or network.

42. What is PositionalDataSource in the context of Android Architecture Components?
    Answer: PositionalDataSource is a DataSource class for data that can be accessed by position or count. It is useful
    when you have a countable static data set to load, such as from a database query.

43. What is ItemKeyedDataSource in the context of Android Architecture Components?
    Answer: ItemKeyedDataSource is a DataSource class for data that is fetched based on keys. It is useful when you need
    to use data from item N-1 to fetch item N.

44. What is PageKeyedDataSource in the context of Android Architecture Components?
    Answer: PageKeyedDataSource is a DataSource class for data that is fetched in pages. It is useful when there are
    keys for next or previous pages, such as in an API.

45. What is BoundaryCallback in the context of Android Architecture Components?
    Answer: BoundaryCallback is a callback for when a PagedList has reached the end of available data. It is used to
    signal that you should fetch more data.

46. What is MutableStateFlow in the context of Android Architecture Components?
    Answer: MutableStateFlow is a state holder observable flow that emits the current and new state updates to its
    collectors. It is part of Kotlin’s coroutines library.

47. What is StateFlow in the context of Android Architecture Components?
    StateFlow is a state holder observable flow that emits the current and new state updates to its collectors. It is
    part of Kotlin’s coroutines library.

48. What is SharedFlow in the context of Android Architecture Components?
    Answer: SharedFlow is a hot flow that shares emitted values among all its collectors. It is part of Kotlin’s
    coroutines library.

49. What is ConflatedBroadcastChannel in the context of Android Architecture Components?
    Answer: ConflatedBroadcastChannel is a BroadcastChannel that immediately consumes and conflates its elements upon
    sending, so that the receiver always gets the most recently sent element. It is part of Kotlin’s coroutines library.

50. What is MutableSharedFlow in the context of Android Architecture Components?
    Answer: MutableSharedFlow is a SharedFlow that provides functions to emit values. It is part of Kotlin’s coroutines
    library.

51. What is CoroutineScope in the context of Android Architecture Components?
    Answer: CoroutineScope is an interface that defines a scope for launching coroutines. All coroutine builders are
    extensions on CoroutineScope and inherit its coroutine context to automatically propagate both context elements and
    cancellation.

52. What is CoroutineDispatcher in the context of Android Architecture Components?
    Answer: CoroutineDispatcher is an interface in Kotlin’s coroutines library that dispatches coroutine execution to a
    specific thread.

53. What is Dispatchers.Main in the context of Android Architecture Components?
    Answer: Dispatchers.Main is a CoroutineDispatcher that is confined to the Main thread operating with UI objects. It
    is typically used for UI-related tasks.

54. What is Dispatchers.IO in the context of Android Architecture Components?
    Answer: Dispatchers.IO is a CoroutineDispatcher that is designed for offloading blocking IO tasks to a shared pool
    of threads.

55. What is Dispatchers.Default in the context of Android Architecture Components?
    Answer: Dispatchers.Default is a CoroutineDispatcher that is optimized for CPU-intensive work, such as sorting large
    lists, doing complex calculations and similar tasks.

56. What is suspend keyword in the context of Android Architecture Components?
    Answer: suspend is a keyword in Kotlin that is used to mark a function or method as a suspending function. These
    functions can suspend the execution of a coroutine without blocking the underlying thread.

57. What is CoroutineContext in the context of Android Architecture Components?
    Answer: CoroutineContext is a set of various elements that define the behavior of a coroutine. It includes elements
    like the job of the coroutine and the dispatcher that the coroutine uses.

58. What is Job in the context of Android Architecture Components?
    Answer: Job is an interface that represents a cancellable piece of work. It has a life-cycle and can form structured
    concurrency hierarchies.

59. What is SupervisorJob in the context of Android Architecture Components?
    Answer: SupervisorJob is a type of Job that does not propagate cancellation to its children. This is useful when you
    have a group of coroutines that should be independent of each other.

60. What is CoroutineExceptionHandler in the context of Android Architecture Components?
    Answer: CoroutineExceptionHandler is an optional element of the CoroutineContext that is invoked when a coroutine in
    the context throws an exception.

61. What is CoroutineName in the context of Android Architecture Components?
    Answer: CoroutineName is a name of the coroutine that is included into the thread name that is executing this
    coroutine. It is defined in the CoroutineContext of the coroutine.

62. What is CoroutineStart in the context of Android Architecture Components?
    Answer: CoroutineStart is an option that can be passed to coroutine builders like launch and async to determine when
    the coroutine should be started.

63. What is launch in the context of Android Architecture Components?
    Answer: launch is a coroutine builder that is used to start a coroutine. It creates a new coroutine and returns a
    reference to it as a Job.

64. What is async in the context of Android Architecture Components?
    Answer: async is a coroutine builder that is used to start a coroutine for concurrent work. It creates a new
    coroutine and returns its future result as an implementation of Deferred<T>.

65. What is runBlocking in the context of Android Architecture Components?
    Answer: runBlocking is a coroutine builder that blocks the current thread until its coroutine body and all its
    children complete execution.

66. What is withContext in the context of Android Architecture Components?
    Answer: withContext is a suspending function that changes the CoroutineDispatcher for the execution of the block of
    code within its scope.

67. What is Deferred in the context of Android Architecture Components?
    Answer: Deferred is a non-blocking cancellable future — it is a Job with a result.

68. What is select expression in the context of Android Architecture Components?
    Answer: select expression is used in Kotlin coroutines to select one of multiple suspending functions that are ready
    for execution.

69. What is yield function in the context of Android Architecture Components?
    Answer: yield is a suspending function that is used to give other coroutines a chance to execute.

70. What is join function in the context of Android Architecture Components?
    Answer: join is a suspending function that is used to wait for a coroutine to complete without blocking the current
    thread.

71. What is cancel function in the context of Android Architecture Components?
    Answer: cancel function is used to cancel a coroutine job.

72. What is isActive property in the context of Android Architecture Components?
    isActive is a property of a coroutine’s Job that returns true if the job is still active (has not completed and was
    not cancelled).

73. What is isCompleted property in the context of Android Architecture Components?
    Answer: isCompleted is a property of a coroutine’s Job that returns true if the job has completed for any reason.

74. What is isCancelled property in the context of Android Architecture Components?
    Answer: isCancelled is a property of a coroutine’s Job that returns true if the job was cancelled for any reason.

75. What is children property in the context of Android Architecture Components?
    Answer: children is a property of a coroutine’s Job that returns a sequence of its immediate children.

76. What is cancelAndJoin function in the context of Android Architecture Components?
    Answer: cancelAndJoin is a suspending function that cancels the job and waits for its completion.

77. What is ensureActive function in the context of Android Architecture Components?
    Answer: ensureActive is a function that checks whether the coroutine’s job is still active. If not, it throws a
    CancellationException.

78. What is handleCoroutineException function in the context of Android Architecture Components?
    Answer: handleCoroutineException is a function that handles uncaught exceptions in coroutines. It’s typically used
    in a CoroutineExceptionHandler.

79. What is NonCancellable in the context of Android Architecture Components?
    Answer: NonCancellable is a job that cannot be cancelled. It’s used when you need to make a section of your code
    non-cancellable.

80. What is SupervisorScope in the context of Android Architecture Components?
    Answer: SupervisorScope is a scope that does not propagate its children’s cancellation. It’s used when you need to
    make a section of your code independent in terms of cancellation.

81. What is coroutineScope function in the context of Android Architecture Components?
    Answer: coroutineScope is a suspending function that creates a new coroutine scope and does not complete until all
    launched children complete.

82. What is supervisorScope function in the context of Android Architecture Components?
    Answer: supervisorScope is a suspending function that creates a new supervisor scope. It’s used when you need to
    make a section of your code independent in terms of cancellation.

83. What is launchIn function in the context of Android Architecture Components?
    Answer: launchIn is an extension function on Flow that launches the collection of the flow in the provided coroutine
    scope.

84. What is catch operator in the context of Android Architecture Components?
    Answer: catch is an operator in Kotlin’s Flow API that catches exceptions from upstream and emits them as values
    downstream.

85. What is collect function in the context of Android Architecture Components?
    Answer: collect is a terminal operator in Kotlin’s Flow API that collects the values emitted by the flow.

86. What is flowOn operator in the context of Android Architecture Components?
    Answer: flowOn is an operator in Kotlin’s Flow API that changes the context of the flow upstream of it.

87. What is map operator in the context of Android Architecture Components?
    Answer: map is an operator in Kotlin’s Flow API that transforms the values emitted by the flow.

88. What is filter operator in the context of Android Architecture Components?
    Answer: filter is an operator in Kotlin’s Flow API that filters values emitted by the flow based on a predicate.

89. What is reduce operator in the context of Android Architecture Components?
    Answer: reduce is a terminal operator in Kotlin’s Flow API that accumulates the values emitted by the flow into a
    single value.

90. What is scan operator in the context of Android Architecture Components?
    Answer: scan is an operator in Kotlin’s Flow API that accumulates the values emitted by the flow and emits each
    intermediate result.

91. What is take operator in the context of Android Architecture Components?
    Answer: take is an operator in Kotlin’s Flow API that only takes the first n values emitted by the flow.

92. What is buffer operator in the context of Android Architecture Components?
    Answer: buffer is an operator in Kotlin’s Flow API that allows the flow to asynchronously collect values and send
    them to a buffer from which they are consumed.

93. What is combine operator in the context of Android Architecture Components?
    Answer: combine is an operator in Kotlin’s Flow API that combines the latest values of several flows together
    through a combining function.

94. What is zip operator in the context of Android Architecture Components?
    Answer: zip is an operator in Kotlin’s Flow API that combines two flows into pairs. It waits for values from both
    flows and combines them as soon as both are available.

95. What is onEach operator in the context of Android Architecture Components?
    Answer: onEach is an operator in Kotlin’s Flow API that performs a given action on each value of the flow.

96. What is catch operator in the context of Android Architecture Components?
    Answer: catch is an operator in Kotlin’s Flow API that catches exceptions from the upstream flow and emits them as
    values downstream.

97. What is flatMapConcat operator in the context of Android Architecture Components?
    Answer: flatMapConcat is an operator in Kotlin’s Flow API that transforms the original flow into multiple flows, and
    then flattens these flows into a single flow.

98. What is flatMapMerge operator in the context of Android Architecture Components?
    Answer: flatMapMerge is an operator in Kotlin’s Flow API that transforms the original flow into multiple flows, and
    then merges these flows into a single flow.

99. What is flatMapLatest operator in the context of Android Architecture Components?
    Answer: flatMapLatest is an operator in Kotlin’s Flow API that transforms the original flow into multiple flows,
    and then switches to the latest flow as soon as it is emitted.

100. What is StateFlow in the context of Android Architecture Components?
     Answer: StateFlow is a state holder observable flow that emits the current and new state updates to its collectors.
     It is part of Kotlin’s coroutines library.

101. What is SharedFlow in the context of Android Architecture Components?
     Answer: SharedFlow is a hot flow that shares emitted values among all its collectors. It is part of Kotlin’s
     coroutines library.