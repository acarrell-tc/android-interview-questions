Advanced Android Interview Questions
====================================

### 1. What is the significance of the .dex file?

Android programs are compiled into a .dex file (Dalvik Executable file) by DVM, which are then zipped into a single .apk
file on the device. The data stored in these DEX files includes compiled code that locates and initializes other program
files of the associated application required to run the program. So that these DEX files are used to initialize and
execute applications developed for the Android mobile OS.

### 2. Describe about FragmentPagerAdapter and FragmentStatePagerAdapter?

- FragmentPagerAdapter: Each fragment visited by the user will be stored in the memory but the view will be destroyed.
  When the page is revisited, then the view will be created not the instance of the fragment. Since API 27
  FragmentPagerAdapter is deprecated.
- FragmentStatePagerAdapter: Here, the fragment instance will be destroyed when it is not visible to the user, except
  the saved state of the fragment. Since API 27 FragmentPagerAdapter is deprecated.

### 3. What is a Service in Android?

A Service is a component that runs in the background to perform long-running operations such as playing music,
downloading content or updating a remote database without any user interaction. It doesn’t have any UI (user interface).
The service runs in the background indefinitely even if application is destroyed. To avoid bad user experience Service
plays a vital role. If developers don’t handle long running operations properly, they slowly clutter the main thread,
creating memory leaks and inconsistencies in the results. To avoid this, we can Start service by creating a new
background thread or use an IntentService that can do work in background

### 4. Explain different types of services in Android?

There are the three different types of services:

- Foreground Service: A foreground service performs some operation that is noticeable to the user. For example,
  downloading a file, the user can keep track of the progress in downloading and can also pause and resume the process.
  Foreground services continue running even when the user isn’t interacting with the app.
- Background Service: A background service performs an operation that isn’t directly noticed by the user. Schedule
  syncing of data is the best example of this type of service. However, there are restrictions to use background
  services from Android API 26 and above.
- Bound Service: This type of android service is bound when an application component binds to it by calling
  bindService(). The client can also unbind the service by calling the unbindService() method.

In Android, A bound service offers a client-server interface that allows components to interact with the service, send
requests, receive results, and even do so across processes with interprocess communication (IPC). A bound service runs
only as long as another application component is bound to it. Multiple components can bind to the service at once, but
when all of them unbind, the service is destroyed by the system.

### 5. How to Stop a Service?

To stop a service from an activity user have to call stopService(Intent intent) method. To Stop a service from itself,
user can call stopSelf() method.

### 6. How to reduce your app size?

- Set minifyEnabled to true
- Set shrinkResources to true
- In developer console using bundle instead of apk
- Convert the images to vector drawables.
- Use the Android Size Analyzer
- Remove unused resources
- Minimize resource use from libraries
- Compress PNG and JPEG files and Use WebP file format
- Use specific screen densities

### 7. When to use a service and when to use a thread?

- Thread: You should use Thread when you want to do any task off the main thread during your app is running (like sound
  of game).
- Service: You should use Service when you want to keep running your operation even your app is in background (like
  music player).

### 8. Explain Sensors in Android.

Android sensors are virtual devices which provide data coming from a set of physical sensors like accelerometers,
gyroscopes, magnetometers, barometer, humidity, pressure, light, proximity and heart rate sensors. Most of the android
devices have built-in sensors that measure motion, orientation, and various environmental condition. The sensors can be
both hardware and software based on nature. There are three prominent categories of sensors in Android devices. They
are:

- Motion Sensors: These sensors consist of gravity, rotational activity, and acceleration sensors which measure the
  rotation of the device or the acceleration, etc.
- Position Sensor: It is used for measuring the physical position of the Android device. This category includes
  orientation sensors and magnetometers.
- Environmental Sensor: It includes sensors that measure temperature, humidity, pressure, illumination and other
  environmental factors. This category includes barometers, photometers, and thermometers.

### 9. What is Android Sensor API?

Using Android Sensor API user can collect raw sensor data. Android sensor API provides many classes and interfaces. Some
of the important classes and interfaces are:

1. SensorManager Class: Sensor manager is used to accessing various sensors present in the device.

2. Sensor Class: The sensor class is used to get information about the sensor such as sensor name, sensor type, sensor
   resolution etc.

3. SensorEvent class: This class is used to find information about the sensor.

4. SensorEventListener interface: This is used to perform some action when sensor accuracy changes.

### 10. What are containers in Android?

Containers are a way to organize a collection of objects, widgets, and other elements. Containers can hold labels,
buttons, fields, or even child containers, etc. For example, if we want a form with labels on the left and fields on the
right, we will need a container. If we have several widgets, we will need a container to have a root element to place
the widgets inside.

Containers are also useful for managing views. Android provides a collection of view classes that serve as containers
for views. These container classes are known as layouts, which are defined in the form of XML files that cannot be
changed from our code during execution. Android SDK provide different layout managers. They are LinearLayout,
RelativeLayout, FrameLayout, AbsoluteLayout, GridLayout, and TableLayout.

### 11. What is the difference between a layout and a container in Android?

A container in android is a view which used to contain other views. Android provides a set of view classes that act as
containers for views. These container classes are known as layouts, and as the name suggests, they decide the
organization, size, and position of their children views.

Basically, Layouts in android are containers for other items known as Views, which are displayed on the screen. Layouts
help manage and arrange views as well. Layouts are defined in the form of XML files that cannot be changed by our code
during runtime.

### 12. What is the importance of setting up permission in Android application development?

If the code is accessible to anyone and without restrictions, there may be a situation where the code is compromised,
resulting in defect leakage. Permission allows certain restrictions to be imposed primarily to protect data and code, so
that the code becomes available to authorized users only.

### 13. Describe the different data storage options available on the Android platform.

There are variety of data storage options are available in android which can be used depending on the need of the user.
The storage options are:

- SharedPreference: Stores data in XML files
- Internal Storage: Stores data in the device file system where it cannot be read by other applications
- SQLite: Stores structured data in the private database
- External Storage: Stores data in the file system but it can be accessed to all apps in the device

### 14. What is ADB in Android?

ADB refers Android Debug Bridge. ADB is a command-line tool that allows you to communicate with a device The main
function of ADB is to allow and control the communication process towards the emulator port and get a response from it.
It helps you perform different actions like installing or debugging a device and run various commands on a device by
providing access to a Unix shell.

### 15. What is an “Emulator” in Android?

The Android emulator is an Android Virtual Device (AVD), which represents a specific Android device. You can use an
Android emulator as a target platform to run and test your Android applications on your PC. This way, it becomes easier
for the developers to write and test different codes for the application. The process of debugging also possible via
emulators.

### 16. What is a singleton class in Android?

A singleton class is a class which can create only an object/instance that can be shared by all other classes.

### 17. What database is used in Android? How it is different from client-server database management systems?

In Android, SQLite is used which is an open-source relational database. The SQLite engine is server less, transactional,
and also self-contained. The SQLite engine is integrally linked with the application instead of the client-server
relationship of most database management systems. The library can be called dynamically and it can make use of simple
function calls that reduce latency in database access.

### 18. How are escape characters used as attribute?

Escape characters are preceded by double backslashes. For example, a newline character is created using ‘\\n’

### 19. Are there any critical loops while monitoring an activity?

Yup, there are three key loops when monitoring an activity. They are:

- Loop 1, Entire Lifetime: The activity happens between onCreate and onDestroy.
- Loop 2, Visible Lifetime: The activity happens between onStart and onStop
- Loop 3, Foreground Lifetime: The activity happens between onResume and onPause

### 20. What are the possible states in which a process is based?

The possible states in which a process is based include the following:

- State 1: Foreground activity
- State 2: Visible activity
- State 3: Background activity
- State 4: Empty activity

### 21. What is the content provider? How it is implemented?

Content provider is one of the primary building blocks of Android applications, which manages access to a central
repository of data. It acts as a standard interface that connects data in one process with code running in another
process. So it can be used to share the data between different applications.

They are responsible for encapsulating the data and providing mechanisms for defining data security. It is implemented
as a subclass of ContentProviderclass and must implement a set of APIs that will enable other applications to perform
transactions.

```java
public class MyContentprovider extends ContentProvider {
    public void onCreate() {
    }
}
```

### 22. What is HandlerThread?

HandlerThread is a Handy class to start a thread that has a Looper.

### 23. What is a Looper?

A Looper is a class used to loop through the Message Queue attached to the Thread. Any thread consists of only one
looper. We can access message queue of current thread by using Looper.myQueue().

By default, a thread halts when the execution completes. But, for Example, if we take Android’s Main thread, it should
not halt upon execution.

Normally thread cannot be reused once its job is completed. But thread with Looper is kept alive until you call quit
method so you don’t need to create a new instance each time you want to run a job in background.

Rather it should loop through the runnables(Messages) that its assigned in order to work properly.

### 24. What is a Message Queue?

MessageQueue is a queue that has list of messages which should be processed. Android maintains a MessageQueue on the
main thread.

### 25. What is a Message?

Message contains a description and arbitrary data object that can be sent to a Handler. It’s used to process / send some
data across threads.

### 26. What are Processes in Android?

Every time an Android App starts, the Android System creates a New Process for this Application with a Single thread of
Execution. By default all the components of the same application runs in the same process. While most apps do not change
this behavior, some apps like games, might want to run in different processes. Then we can use android:process attribute
in our AndroidManifest.xml to specify the process name.

### 27. What is a RetainFragment / Headless Fragment?

Generally, Fragments are destroyed and recreated along with their parent Activity’s whenever a configuration change
occurs. Calling setRetainInstance(true) allows us to bypass this destroy-and-recreate cycle, notifying the system to
retain the current instance of the fragment when the activity is recreated.

### 28. When Intent Service is Useful?

The IntentService can be used in long tasks usually with no communication to Main Thread. If communication is required,
can use Main Thread handler or broadcast intents. Another case of use is when callbacks are needed (Intent triggered
tasks).

### 29. What are the differences between Service and Thread?

- Service is an application component that facilitates an application to run in the background in order to perform
  long-running operations without user interaction. A Thread is a concurrent unit of execution.
- Service exposes few functionalities to other applications by calling Context.bindService(). Google has brought in
  handlers and loopers into threads.
- When an application is killed, service is not killed. When an application is killed, the thread is killed.

### 30. What are Default Resources? How are they useful?

The default resources include the default strings and files. Their absence will result in creating errors on the screen
and could also hinder the running of the downloaded application. They are useful as they are placed as subdirectories
under the project directory, which supports the running of the downloaded application.

### 31. What are the troubleshooting techniques you can follow if an application is crashing frequently?

If an Android application is crashing frequently, you can follow the below-given techniques:

#### Compatibility Check:

It may not be a hardware problem, but more of a software issue. It is not possible normally to test an application for
all kinds of devices and operating systems. There might be a possibility that an application is not compatible with your
OS.

#### Memory Management:

Some apps run perfectly on one mobile device but might crash on other devices. Here processing power, memory management,
and CPU speed are to be taken into account.
Since mobile devices only have a limited amount of memory space, you can free up memory to allow the program to run
smoothly. Check the application memory requirements if the application crashes constantly.
If an application is frequently crashing, you can delete the application’s data, which will clear its cache memory and
allow some free space on your device and might boost the app’s performance.

### 32. How do you create a Memory Leak in Android?

By passing the context to static block (class or method), we can create a Memory Leak.

### 33. How do you identify a Memory Leak in Android?

By using Profiler in Android Studio or by using LeakCanary Library in Android.

### 34. How do you avoid a Memory Leak in Android?

By making the objects eligible for GC (Garbage Collection) after a class (Activity or Fragment) is destroyed. We can
also use Weak References like WeakHashMaps to loosely hold the data and make it easily available to GC.

### 35. Can you explain how garbage collection works?

The garbage collector will automatically release the memory that was used by an object when it is no longer used by the
program, preventing memory leaks. The garbage collector runs periodically, so it may not happen immediately when the
object is no longer needed. The GC mechanism works by tracking object references and periodically scanning the heap for
unreachable objects. Once identified, these objects are marked for removal, and their memory space is reclaimed during
the next sweep phase. It helps maintain a smooth user experience by ensuring efficient use of available memory
resources.

### 36. What are the potential downsides of Garbage Collection?

Potential drawbacks of garbage collection are:

1. Performance overhead: The GC process consumes CPU cycles, which can lead to reduced app performance, especially if it
   runs frequently or takes too long.
2. Pauses: During GC, application threads may be paused, causing noticeable delays or stuttering in the user interface.
3. Fragmentation: Repeated GC cycles can cause memory fragmentation, making it difficult to allocate large contiguous
   blocks of memory.

#### How to avoid downsides of Garbage Collection?

Developers need to optimize their code by minimizing object allocations, using appropriate data structures, and
employing caching techniques when possible to avoid drawbacks of Garbage Collection.

### 37. How to fix memory issues in Android.

- Optimize data structures and algorithms to reduce memory footprint.
- Implement caching strategies with proper eviction policies.
- Use appropriate Android components (e.g., ViewModel) to handle configuration changes without leaking context.
- Compress images and use BitmapFactory.Options.inSampleSize to load smaller versions of bitmaps.
- Employ WeakReference/SoftReference when necessary to allow garbage collection of unused objects.

### 38. When you should use weak references or soft references to manage memory in Android applications?

When you want to maintain a reference to an object without preventing it from being garbage collected, you should use
weak references. They’re beneficial in scenarios like caching, where the data can be recreated if needed.

On the other hand, Soft references are ideal for memory-sensitive caches. They hold onto their referents more strongly
than weak references but still allow garbage collection under low-memory conditions. This ensures better retention of
cached data while maintaining responsiveness during memory pressure.

### 39. Describe drawbacks of weak references or soft references.

- Weakly referenced objects may be collected too soon, causing performance issues.
- However, soft references can cause longer GC pauses and make it harder to predict when objects will be reclaimed.

### 40. How to handle crashing of AsyncTask during screen rotation?

One way is by cancelling the AsyncTask by using cancel() method on its instance. It will call onCancelled() method of
AsyncTask where we can do some clean-up activities like hiding progress bar etc. The best way to handle AsyncTask crash
is to create a RetainFragment :

```java
public class RetainFragExampleActivity extends Activity {

    @Override
    protected void onCreate(Bundle savedInstanceState) {
        super.onCreate(savedInstanceState);
        setContentView(R.layout.activity_my);

        Button b = (Button) findViewById(R.id.aaa);
        b.setOnClickListener(new View.OnClickListener() {
            @Override
            public void onClick(View v) {
                RetainFragment retainFragment =
                        RetainFragment.getInstance(getFragmentManager());
                retainFragment.loadAsync();
            }
        });
    }

    private void handleResponse(String response) {
        // do something with the response...
    }

    public static class RetainFragment extends Fragment {
        private static final String TAG = "RetainFragment";

        private RetainFragment() {
        }

        public static RetainFragment getInstance(FragmentManager fm) {
            RetainFragment fragment = (RetainFragment) fm.findFragmentByTag(TAG);
            if (fragment == null) {
                fragment = new RetainFragment();
                fm.beginTransaction().add(fragment, TAG).commit();
            }
            return fragment;
        }

        @Override
        public void onCreate(Bundle savedInstanceState) {
            super.onCreate(savedInstanceState);
            setRetainInstance(true);
        }

        public void loadAsync() {
            new AsyncTask<Void, Void, String>() {
                @Override
                protected String doInBackground(Void... params) {
                    // Do some work...
                    return null;
                }

                @Override
                protected void onPostExecute(String response) {
                    MyActivity myActivity = (MyActivity) getActivity();
                    if (myActivity != null) {
                        myActivity.handleResponse(response);
                    }
                }
            }.execute();
        }
    }
}
```

We can also avoid this crash by using 2 Alternatives — 1) Using RxJava by subscribing and unsubscribing at onResume()
and onPause() methods respectively, 2) Using LiveData — lifecycle aware component.

Sources: 
- https://medium.com/@md.zakirhossain/advanced-android-interview-questions-and-answer-part-01-72a5fe5a3c82
- https://medium.com/@md.zakirhossain/advanced-android-interview-questions-and-answer-part-02-f48a749bda15
- https://medium.com/@md.zakirhossain/advanced-android-interview-questions-and-answer-part-03-handle-application-crash-and-memory-1fa43613e422