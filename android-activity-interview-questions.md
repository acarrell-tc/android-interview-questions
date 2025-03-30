Android Activity Interview Questions
====================================

* [What happens to an Activity when the Home button is pressed?](#what-happens-to-an-activity-when-the-home-button-is-pressed)
* [What happens to an Activity when the Back button is pressed?](#what-happens-to-an-activity-when-the-back-button-is-pressed)
* [How can you intercept the Back button press in an Activity?](#how-can-you-intercept-the-back-button-press-in-an-activity)
* [What is the purpose of the onUserLeaveHint() method?](#what-is-the-purpose-of-the-onuserleavehint-method)
* [How can you launch an Activity when the user presses the Home button?](#how-can-you-launch-an-activity-when-the-user-presses-the-home-button)
* [How can you prevent the Back button from destroying your Activity?](#how-can-you-prevent-the-back-button-from-destroying-your-activity)
* [What happens to an Activity when the device screen is turned off?](#what-happens-to-an-activity-when-the-device-screen-is-turned-off)
* [What happens to an Activity when a phone call is received?](#what-happens-to-an-activity-when-a-phone-call-is-received)
* [What happens to an Activity when a configuration change occurs (like rotation)?](#what-happens-to-an-activity-when-a-configuration-change-occurs-like-rotation)
* [How can you retain an Activity’s state during a configuration change?](#how-can-you-retain-an-activitys-state-during-a-configuration-change)
* [What happens to an Activity when another Activity is launched on top?](#what-happens-to-an-activity-when-another-activity-is-launched-on-top)
* [How can you ensure that an Activity is not destroyed when the user rotates the screen?](#how-can-you-ensure-that-an-activity-is-not-destroyed-when-the-user-rotates-the-screen)
* [What is the onUserLeaveHint() method in Android?](#what-is-the-onuserleavehint-method-in-android)
* [What is the difference between onPause() and onStop()?](#what-is-the-difference-between-onpause-and-onstop)
* [How can you save the state of an Activity before it gets destroyed?](#how-can-you-save-the-state-of-an-activity-before-it-gets-destroyed)
* [What is the onRestoreInstanceState() method in Android?](#what-is-the-onrestoreinstancestate-method-in-android)
* [What happens to an Activity when the device goes to sleep or when the lock screen appears?](#what-happens-to-an-activity-when-the-device-goes-to-sleep-or-when-the-lock-screen-appears)
* [What happens to an Activity when a dialog appears?](#what-happens-to-an-activity-when-a-dialog-appears)
* [What happens to an Activity when you navigate to a different app using the Recent Apps list?](#what-happens-to-an-activity-when-you-navigate-to-a-different-app-using-the-recent-apps-list)
* [What is the onActivityResult() method in Android?](#what-is-the-onactivityresult-method-in-android)
* [What is the onBackPressed() method in Android?](#what-is-the-onbackpressed-method-in-android)
* [What is the onUserLeaveHint() method in Android?](#what-is-the-onuserleavehint-method-in-android-1)
* [What is the onPause() method in Android?](#what-is-the-onpause-method-in-android)
* [When is onStop() method called in Android?](#when-is-onstop-method-called-in-android)
* [What is the onDestroy() method in Android?](#what-is-the-ondestroy-method-in-android)
* [What is the onRestart() method in Android?](#what-is-the-onrestart-method-in-android)
* [What is the onResume() method in Android?](#what-is-the-onresume-method-in-android)
* [What is the onStart() method in Android?](#what-is-the-onstart-method-in-android)
* [What is the onCreate() method in Android?](#what-is-the-oncreate-method-in-android)
* [What is the onSaveInstanceState() method in Android?](#what-is-the-onsaveinstancestate-method-in-android)
* [What is the onRestoreInstanceState() method in Android?](#what-is-the-onrestoreinstancestate-method-in-android-1)
* [What is the onPostCreate() method in Android?](#what-is-the-onpostcreate-method-in-android)
* [What is the onPostResume() method in Android?](#what-is-the-onpostresume-method-in-android)
* [What is the onTitleChanged() method in Android?](#what-is-the-ontitlechanged-method-in-android)
* [What is the onChildTitleChanged() method in Android?](#what-is-the-onchildtitlechanged-method-in-android)
* [What is the onKeyDown() method in Android?](#what-is-the-onkeydown-method-in-android)
* [What is the onKeyLongPress() method in Android?](#what-is-the-onkeylongpress-method-in-android)
* [What is the onKeyMultiple() method in Android?](#what-is-the-onkeymultiple-method-in-android)
* [What is the onKeyUp() method in Android?](#what-is-the-onkeyup-method-in-android)
* [What is the onKeyShortcut() method in Android?](#what-is-the-onkeyshortcut-method-in-android)
* [What is the onTouchEvent() method in Android?](#what-is-the-ontouchevent-method-in-android)
* [What is the onTrackballEvent() method in Android?](#what-is-the-ontrackballevent-method-in-android)
* [What is the onGenericMotionEvent() method in Android?](#what-is-the-ongenericmotionevent-method-in-android)
* [What is the onUserInteraction() method in Android?](#what-is-the-onuserinteraction-method-in-android)
* [What is the onWindowAttributesChanged() method in Android?](#what-is-the-onwindowattributeschanged-method-in-android)
* [What is the onWindowFocusChanged() method in Android?](#what-is-the-onwindowfocuschanged-method-in-android)
* [What is the onCreateThumbnail() method in Android?](#what-is-the-oncreatethumbnail-method-in-android)
* [What is the onCreateDescription() method in Android?](#what-is-the-oncreatedescription-method-in-android)
* [What is the onProvideAssistData() method in Android?](#what-is-the-onprovideassistdata-method-in-android)
* [What is the onProvideKeyboardShortcuts() method in Android?](#what-is-the-onprovidekeyboardshortcuts-method-in-android)
* [What is an Activity in Android?](#what-is-an-activity-in-android)
* [What is the lifecycle of an Activity?](#what-is-the-lifecycle-of-an-activity)
* [What is the difference between onPause() and onStop()?](#what-is-the-difference-between-onpause-and-onstop-1)
* [What is an Intent?](#what-is-an-intent)
* [What is the difference between startActivity() and startActivityForResult()?](#what-is-the-difference-between-startactivity-and-startactivityforresult)
* [What is a Task in Android?](#what-is-a-task-in-android)
* [What is the onSaveInstanceState() method?](#what-is-the-onsaveinstancestate-method)
* [What is a Fragment?](#what-is-a-fragment)
* [What is the difference between a Fragment and an Activity?](#what-is-the-difference-between-a-fragment-and-an-activity)
* [What is Context in Android?](#what-is-context-in-android)
* [What is onActivityResult() in Android?](#what-is-onactivityresult-in-android)
* [What is the difference between finish() and onDestroy()?](#what-is-the-difference-between-finish-and-ondestroy)
* [What is onBackPressed()?](#what-is-onbackpressed)
* [What is onConfigurationChanged()?](#what-is-onconfigurationchanged)
* [What is the role of the AndroidManifest.xml file?](#what-is-the-role-of-the-androidmanifestxml-file)
* [What is an Activity stack?](#what-is-an-activity-stack)
* [What is startActivityFromChild()?](#what-is-startactivityfromchild)
* [What is startActivityFromFragment()?](#what-is-startactivityfromfragment)
* [What is singleTask launch mode?](#what-is-singletask-launch-mode)
* [What is singleInstance launch mode?](#what-is-singleinstance-launch-mode)
* [What is onNewIntent() in Android?](#what-is-onnewintent-in-android)
* [What is onUserLeaveHint() in Android?](#what-is-onuserleavehint-in-android)
* [What is onUserInteraction() in Android?](#what-is-onuserinteraction-in-android)
* [What is onWindowFocusChanged() in Android?](#what-is-onwindowfocuschanged-in-android)
* [What is onAttachedToWindow() in Android?](#what-is-onattachedtowindow-in-android)
* [What is onDetachedFromWindow() in Android?](#what-is-ondetachedfromwindow-in-android)
* [What is onContentChanged() in Android?](#what-is-oncontentchanged-in-android)
* [What is onCreateDialog() in Android?](#what-is-oncreatedialog-in-android)
* [What is onPrepareDialog() in Android?](#what-is-onpreparedialog-in-android)
* [What is onSearchRequested() in Android?](#what-is-onsearchrequested-in-android)
* [What is onOptionsItemSelected() in Android?](#what-is-onoptionsitemselected-in-android)
* [What is onOptionsMenuClosed() in Android?](#what-is-onoptionsmenuclosed-in-android)
* [What is onPrepareOptionsMenu() in Android?](#what-is-onprepareoptionsmenu-in-android)
* [What is onPostCreate() in Android?](#what-is-onpostcreate-in-android)
* [What is onPostResume() in Android?](#what-is-onpostresume-in-android)
* [What is onTitleChanged() in Android?](#what-is-ontitlechanged-in-android)
* [What is onChildTitleChanged() in Android?](#what-is-onchildtitlechanged-in-android)
* [What is onKeyDown() in Android?](#what-is-onkeydown-in-android)
* [What is onKeyLongPress() in Android?](#what-is-onkeylongpress-in-android)
* [What is onKeyMultiple() in Android?](#what-is-onkeymultiple-in-android)
* [What is onKeyUp() in Android?](#what-is-onkeyup-in-android)
* [What is onKeyShortcut() in Android?](#what-is-onkeyshortcut-in-android)
* [What is onTouchEvent() in Android?](#what-is-ontouchevent-in-android)
* [What is onTrackballEvent() in Android?](#what-is-ontrackballevent-in-android)
* [What is onGenericMotionEvent() in Android?](#what-is-ongenericmotionevent-in-android)
* [What is onUserInteraction() in Android?](#what-is-onuserinteraction-in-android-1)
* [What is onWindowAttributesChanged() in Android?](#what-is-onwindowattributeschanged-in-android)
* [What is onWindowFocusChanged() in Android?](#what-is-onwindowfocuschanged-in-android-1)
* [What is onCreateThumbnail() in Android?](#what-is-oncreatethumbnail-in-android)
* [What is onCreateDescription() in Android?](#what-is-oncreatedescription-in-android)
* [What is onProvideAssistData() in Android?](#what-is-onprovideassistdata-in-android)
* [What is onProvideKeyboardShortcuts() in Android?](#what-is-onprovidekeyboardshortcuts-in-android)
* [What is onEnterAnimationComplete() in Android?](#what-is-onenteranimationcomplete-in-android)
* [What is onTopResumedActivityChanged() in Android?](#what-is-ontopresumedactivitychanged-in-android)
* [What is onVisibleBehindCanceled() in Android?](#what-is-onvisiblebehindcanceled-in-android)
* [What is onActionModeFinished() in Android?](#what-is-onactionmodefinished-in-android)
* [What is onActionModeStarted() in Android?](#what-is-onactionmodestarted-in-android)
* [What is onAttachedToWindow() in Android?](#what-is-onattachedtowindow-in-android-1)
* [What is onDetachedFromWindow() in Android?](#what-is-ondetachedfromwindow-in-android-1)
* [What is onWindowAttributesChanged() in Android?](#what-is-onwindowattributeschanged-in-android-1)
* [What is onWindowFocusChanged() in Android?](#what-is-onwindowfocuschanged-in-android-2)
* [What is onCreateThumbnail() in Android?](#what-is-oncreatethumbnail-in-android-1)
* [What is onCreateDescription() in Android?](#what-is-oncreatedescription-in-android-1)
* [What is onProvideAssistData() in Android?](#what-is-onprovideassistdata-in-android-1)
* [What is onProvideKeyboardShortcuts() in Android?](#what-is-onprovidekeyboardshortcuts-in-android-1)
* [What is onEnterAnimationComplete() in Android?](#what-is-onenteranimationcomplete-in-android-1)
* [What is onTopResumedActivityChanged() in Android?](#what-is-ontopresumedactivitychanged-in-android-1)
* [What is onVisibleBehindCanceled() in Android?](#what-is-onvisiblebehindcanceled-in-android-1)
* [What is onActionModeFinished() in Android?](#what-is-onactionmodefinished-in-android-1)
* [What is onActionModeStarted() in Android?](#what-is-onactionmodestarted-in-android-1)
* [What is onAttachedToWindow() in Android?](#what-is-onattachedtowindow-in-android-2)
* [What is onDetachedFromWindow() in Android?](#what-is-ondetachedfromwindow-in-android-2)
* [What is onWindowAttributesChanged() in Android?](#what-is-onwindowattributeschanged-in-android-2)
* [What is onWindowFocusChanged() in Android?](#what-is-onwindowfocuschanged-in-android-3)
* [What is onCreateThumbnail() in Android?](#what-is-oncreatethumbnail-in-android-2)
* [What is onCreateDescription() in Android?](#what-is-oncreatedescription-in-android-2)
* [What is onProvideAssistData() in Android?](#what-is-onprovideassistdata-in-android-2)
* [What is onProvideKeyboardShortcuts() in Android?](#what-is-onprovidekeyboardshortcuts-in-android-2)
* [What is onEnterAnimationComplete() in Android?](#what-is-onenteranimationcomplete-in-android-2)
* [What is onTopResumedActivityChanged() in Android?](#what-is-ontopresumedactivitychanged-in-android-2)
* [What is onVisibleBehindCanceled() in Android?](#what-is-onvisiblebehindcanceled-in-android-2)
* [What is onActionModeFinished() in Android?](#what-is-onactionmodefinished-in-android-2)
* [What is onActionModeStarted() in Android?](#what-is-onactionmodestarted-in-android-2)
* [What is onAttachedToWindow() in Android?](#what-is-onattachedtowindow-in-android-3)
* [What is onDetachedFromWindow() in Android?](#what-is-ondetachedfromwindow-in-android-3)
* [What is onWindowAttributesChanged() in Android?](#what-is-onwindowattributeschanged-in-android-3)
* [What is onWindowFocusChanged() in Android?](#what-is-onwindowfocuschanged-in-android-4)
* [What is onCreateThumbnail() in Android?](#what-is-oncreatethumbnail-in-android-3)
* [What is onCreateDescription() in Android?](#what-is-oncreatedescription-in-android-3)
* [What is onProvideAssistData() in Android?](#what-is-onprovideassistdata-in-android-3)
* [What is onProvideKeyboardShortcuts() in Android?](#what-is-onprovidekeyboardshortcuts-in-android-3)
* [What is onEnterAnimationComplete() in Android?](#what-is-onenteranimationcomplete-in-android-3)
* [What is onTopResumedActivityChanged() in Android?](#what-is-ontopresumedactivitychanged-in-android-3)
* [What is onVisibleBehindCanceled() in Android?](#what-is-onvisiblebehindcanceled-in-android-3)
* [What is onActionModeFinished() in Android?](#what-is-onactionmodefinished-in-android-3)
* [What is onActionModeStarted() in Android?](#what-is-onactionmodestarted-in-android-3)
* [What is onAttachedToWindow() in Android?](#what-is-onattachedtowindow-in-android-4)
* [What is onDetachedFromWindow() in Android?](#what-is-ondetachedfromwindow-in-android-4)
* [What is onWindowAttributesChanged() in Android?](#what-is-onwindowattributeschanged-in-android-4)
* [What is onWindowFocusChanged() in Android?](#what-is-onwindowfocuschanged-in-android-5)

#### What happens to an Activity when the Home button is pressed?

When the Home button is pressed, the current Activity is moved to the background, and the onPause() method is
called, followed by onStop(). The Activity is not destroyed, but it can be killed by the system when memory is needed
elsewhere.

#### What happens to an Activity when the Back button is pressed?

When the Back button is pressed, the current Activity is destroyed, and the previous Activity in the back stack
is resumed. The onPause(), onStop(), and onDestroy() lifecycle methods are called in sequence.

#### How can you intercept the Back button press in an Activity?

You can intercept the Back button press by overriding the onBackPressed() method in your Activity. This allows
you to perform specific actions before the Activity is finished.

#### What is the purpose of the onUserLeaveHint() method?

The onUserLeaveHint() method is called when the user has clicked the Home button or has selected another app
through the Recent Apps list. It allows you to detect that the user is leaving your app.

#### How can you launch an Activity when the user presses the Home button?

Launching an Activity when the Home button is pressed is generally discouraged because it disrupts the standard
navigation flow. However, it can be done by creating a launcher Activity that is started when the HOME intent is fired.

#### How can you prevent the Back button from destroying your Activity?

You can prevent the Back button from destroying your Activity by overriding the onBackPressed() method and not
calling super.onBackPressed() within that method.

#### What happens to an Activity when the device screen is turned off?

When the device screen is turned off, the onPause() method is called, followed by onStop(). The Activity is not
destroyed, but it can be killed by the system when memory is needed elsewhere.

#### What happens to an Activity when a phone call is received?

When a phone call is received, the onPause() method is called, followed by onStop(). The Activity is not
destroyed, but it can be killed by the system when memory is needed elsewhere.

#### What happens to an Activity when a configuration change occurs (like rotation)?

When a configuration change occurs, the Activity is destroyed and recreated. The onPause(), onStop(), and
onDestroy() methods are called, followed by onCreate(), onStart(), and onResume().

#### How can you retain an Activity’s state during a configuration change?

You can retain an Activity’s state during a configuration change by saving the state in the
onSaveInstanceState() method and restoring it in onCreate() or onRestoreInstanceState().

#### What happens to an Activity when another Activity is launched on top?

When another Activity is launched on top, the current Activity is paused and stopped, but not destroyed. The
onPause() and onStop() methods are called in that order.

#### How can you ensure that an Activity is not destroyed when the user rotates the screen?

You can ensure that an Activity is not destroyed during a screen rotation by handling the configuration change
yourself. This can be done by adding android:configChanges="orientation|screenSize" in the Activity’s declaration in the
AndroidManifest.xml.

#### What is the onUserLeaveHint() method in Android?

The onUserLeaveHint() method is called when the user navigates away from the Activity by pressing the Home
button or after a task switch. This method can be overridden to perform actions that should occur only when the user
leaves the app out of their own volition.

#### What is the difference between onPause() and onStop()?

onPause() is called when the Activity is still partially visible, but the user is likely on their way out.
onStop(), on the other hand, is called when the Activity is no longer visible.

#### How can you save the state of an Activity before it gets destroyed?

You can save the state of an Activity before it gets destroyed by implementing the onSaveInstanceState() method
and saving the state information as a Bundle.

#### What is the onRestoreInstanceState() method in Android?

The onRestoreInstanceState() method is called after the onStart() method. It restores the saved state of an
Activity from the Bundle that was saved in the onSaveInstanceState() method.

#### What happens to an Activity when the device goes to sleep or when the lock screen appears?

When the device goes to sleep or when the lock screen appears, the onPause() method is called, followed by
onStop(). The Activity is not destroyed, but it can be killed by the system when memory is needed elsewhere.

#### What happens to an Activity when a dialog appears?

When a dialog appears, the Activity’s onPause() method is called because the Activity loses focus. However,
onStop() is not called because the Activity is still visible behind the dialog.

#### What happens to an Activity when you navigate to a different app using the Recent Apps list?

When you navigate to a different app using the Recent Apps list, the onPause() method is called, followed by
onStop(). The Activity is not destroyed, but it can be killed by the system when memory is needed elsewhere.

#### What is the onActivityResult() method in Android?

The onActivityResult() method is called when an Activity you launched exits, giving you the requestCode you
started it with, the resultCode it returned, and any additional data from it.

#### What is the onBackPressed() method in Android?

The onBackPressed() method is called when the activity has detected the user’s press of the back key. The
default implementation simply finishes the current activity, but you can override this to do whatever you want.

#### What is the onUserLeaveHint() method in Android?

The onUserLeaveHint() method is called when the user navigates away from the activity directly, not because
another activity is launched in front of it. This method is typically used to commit unsaved changes to persistent data.

#### What is the onPause() method in Android?

The onPause() method is called as part of the activity lifecycle when an activity is going into the background,
but has not (yet) been killed. The counterpart to onResume().

#### When is onStop() method called in Android?

onStop() is called when the activity is no longer visible to the user. This may happen because it is being
destroyed, or because another activity (either an existing one or a new one) has been resumed and is covering it.

#### What is the onDestroy() method in Android?

onDestroy() is called before the activity is destroyed. This is the final call that the activity will receive.
It could be called either because the activity is finishing (due to the user completely dismissing the activity or due
to finish() being called on the activity), or because the system is temporarily destroying the activity due to a
configuration change (such as device rotation or multi-window mode).

#### What is the onRestart() method in Android?

onRestart() is called after your activity has been stopped, prior to it being started again. This is followed by
onStart() and onResume().

#### What is the onResume() method in Android?

onResume() is called when the activity will start interacting with the user. At this point, the activity is at
the top of the activity stack, with user input going to it.

#### What is the onStart() method in Android?

onStart() is called when the activity is becoming visible to the user. It is followed by onResume() if the
activity comes to the foreground, or onStop() if it becomes hidden.

#### What is the onCreate() method in Android?

onCreate() is where you initialize your activity. Most importantly, here you will usually call setContentView(
int) with a layout resource defining your UI, and using findViewById(int) to retrieve the widgets in that UI that you
need to interact with programmatically.

#### What is the onSaveInstanceState() method in Android?

onSaveInstanceState() is called to ask the activity to save its current dynamic state, so it can later be
reconstructed in a new instance of its process is restarted. If a new instance of the activity is later created, the
data you place in the Bundle here will be available in the Bundle given to onCreate(Bundle) and onRestoreInstanceState(
Bundle).

#### What is the onRestoreInstanceState() method in Android?

onRestoreInstanceState() is called after onStart() when the activity is being re-initialized from a previously
saved state, as given here in savedInstanceState. Most implementations will simply use onCreate(Bundle) to restore their
state, but it is sometimes convenient to do it here after all of the initialization has been done or to allow subclasses
to decide whether to use your default implementation.

#### What is the onPostCreate() method in Android?

onPostCreate() is called when activity start-up is complete (after onStart() and onRestoreInstanceState(Bundle)
have been called). Applications will generally not implement this method; it is intended for system classes to do final
initialization after application code has run.

#### What is the onPostResume() method in Android?

onPostResume() is called when activity resume is complete (after onResume() has been called). Applications will
generally not implement this method; it is intended for system classes to do final initialization after application code
has run.

#### What is the onTitleChanged() method in Android?

onTitleChanged() is called when the activity’s title changes.

#### What is the onChildTitleChanged() method in Android?

onChildTitleChanged() is called when the title of a child activity changes.

#### What is the onKeyDown() method in Android?

onKeyDown() is called when a key down event has occurred. If you return true, the event is handled and will not
be passed further down the event chain.

#### What is the onKeyLongPress() method in Android?

onKeyLongPress() is called when a key long press event is up. If you return true, the event is handled and will
not be passed further down the event chain.

#### What is the onKeyMultiple() method in Android?

onKeyMultiple() is called when multiple key events have been fired by the system. This is a common occurrence for
keys that are auto-repeated.

#### What is the onKeyUp() method in Android?

onKeyUp() is called when a key up event has occurred. If you return true, the event is handled and will not be
passed further down the event chain.

#### What is the onKeyShortcut() method in Android?

onKeyShortcut() is called when a key shortcut event has occurred. If you return true, the event is handled and
will not be passed further down the event chain.

#### What is the onTouchEvent() method in Android?

onTouchEvent() is a method that gets called when a touch screen event has occurred. If you return true, the
event is handled and will not be passed further down the event chain.

#### What is the onTrackballEvent() method in Android?

onTrackballEvent() is a method that gets called when a trackball motion event has occurred. If you return true, the
event is handled and will not be passed further down the event chain.

#### What is the onGenericMotionEvent() method in Android?

onGenericMotionEvent() is a method that gets called when a generic motion event has occurred. If you return true, the
event is handled and will not be passed further down the event chain.

#### What is the onUserInteraction() method in Android?

onUserInteraction() is a method that gets called when the user interacts with the application. It’s often used
to reset user inactivity timers or to take some action when the user interacts with your application.

#### What is the onWindowAttributesChanged() method in Android?

onWindowAttributesChanged() is a method that gets called when the current Window of the activity has changed
attributes.

#### What is the onWindowFocusChanged() method in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses
focus. This is the best indicator of whether this activity is visible to the user.

#### What is the onCreateThumbnail() method in Android?

onCreateThumbnail() is a method that gets called when the system needs a new thumbnail for this
activity’s task.

#### What is the onCreateDescription() method in Android?

onCreateDescription() is a method that gets called when the system needs a description of this activity’s
current state.

#### What is the onProvideAssistData() method in Android?

onProvideAssistData() is a method that gets called when the system needs additional information to provide
contextual help to the user.

#### What is the onProvideKeyboardShortcuts() method in Android?

onProvideKeyboardShortcuts() is a method that gets called when the system needs to populate the built-in help with
information about your application’s keyboard shortcuts.

#### What is an Activity in Android?

An Activity in Android is a single screen with a user interface. It’s like a window for your application. Each
activity can start another activity to perform different actions.

#### What is the lifecycle of an Activity?

An Activity has several lifecycle methods that are called when the activity’s state changes. These include
onCreate(), onStart(), onResume(), onPause(), onStop(), onDestroy(), and onRestart().

#### What is the difference between onPause() and onStop()?

onPause() is called when the activity is no longer in the foreground but is still visible, while onStop() is
called when the activity is no longer visible.

#### What is an Intent?

An Intent is a messaging object that you can use to request an action from another app component. You can use
intents for a wide variety of tasks, but most often they are used to start another activity.

#### What is the difference between startActivity() and startActivityForResult()?

startActivity() is used to start a new activity without expecting any result back. On the other hand,
startActivityForResult() is used when you expect a result back from the new activity.

#### What is a Task in Android?

A Task is a collection of activities that users interact with when performing a certain job. The activities are
arranged in a stack — the back stack) — in the order in which each activity is opened.

#### What is the onSaveInstanceState() method?

onSaveInstanceState() is a method used to store data before pausing the activity. This data is then passed to
onCreate() if the activity needs to be recreated, allowing the app to restore its state.

#### What is a Fragment?

A Fragment represents a behavior or a portion of user interface in an Activity. You can combine multiple
fragments in a single activity to build a multi-pane UI and reuse a fragment in multiple activities.

#### What is the difference between a Fragment and an Activity?

Both Activity and Fragment are components of Android. However, an Activity is a single, focused thing that the
user can do, while a Fragment is a modular part of an activity, which has its own lifecycle, receives its own input
events, and can be added or removed while the activity is running.

#### What is Context in Android?

Context is an abstract class whose implementation is provided by the Android system. It allows access to
application-specific resources and classes, as well as calls for application-level operations such as launching
activities, broadcasting and receiving intents, etc.

#### What is onActivityResult() in Android?

onActivityResult() is a method you use to receive the result returned by an activity that was started by
startActivityForResult(). It is passed the request code you supplied to startActivityForResult(), a result code it
received from the child activity, and an Intent, which can return result data to the caller.

#### What is the difference between finish() and onDestroy()?

finish() is a method you call to close the current activity. onDestroy(), on the other hand, is a method that is
called by the system to notify you that your activity is being removed from the system memory.

#### What is onBackPressed()?

onBackPressed() is a method called when the activity has detected the user’s press of the back key. The default
implementation simply finishes the current activity, but you can override this to do whatever you want.

#### What is onConfigurationChanged()?

onConfigurationChanged() is a method that gets called by Android system when the device configuration changes
while your activity is running. This can occur, for example, when the device screen orientation changes from landscape
to portrait.

#### What is the role of the AndroidManifest.xml file?

AndroidManifest.xml is a central file in an Android project. It presents essential information about the
application to the Android system, information the system must have before it can run any of the application’s code.

#### What is an Activity stack?

An Activity stack (Back stack) is a stack of activities that are currently running and stacked up together. The activity
at the top of the stack is the activity running on the screen.

#### What is startActivityFromChild()?

startActivityFromChild() is a method you call to start an activity from a child activity. The child activity handles the
onActivityResult() callback.

#### What is startActivityFromFragment()?

startActivityFromFragment() is a method you call to start an activity from a fragment. The fragment handles the
onActivityResult() callback.

#### What is singleTask launch mode?

singleTask is a launch mode where the system creates a new task and instantiates the activity at the root of the
new task. However, if an instance of the activity already exists in a separate task, the system routes the intent to the
existing instance through a call to its onNewIntent() method, rather than creating a new instance.

#### What is singleInstance launch mode?

singleInstance is a launch mode where a new task will always be created and a new instance will be pushed to the
task as the root one. However, if an instance of activity already exists in a separate task, Android will put the
existing task to the foreground.

#### What is onNewIntent() in Android?

onNewIntent() is a method that gets called when the activity receives a new intent while it’s already at the top
of the activity stack. This happens when an activity has set its launchMode to singleTop.

#### What is onUserLeaveHint() in Android?

onUserLeaveHint() is a method that gets called when the user navigates away from the activity directly, not
because another activity is launched in front of it. This method is typically used to commit unsaved changes to
persistent data.

#### What is onUserInteraction() in Android?

onUserInteraction() is a method that gets called whenever the user interacts with the application. It’s often
used to reset user inactivity timers or to take some action when the user interacts with your application.

#### What is onWindowFocusChanged() in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses focus.
This is the best indicator of whether this activity is visible to the user.

#### What is onAttachedToWindow() in Android?

onAttachedToWindow() is a method that gets called when the window has been attached to the window manager. This is a
good place to instantiate objects that contain Paint and Drawable objects that you plan to use with the current window.

#### What is onDetachedFromWindow() in Android?

onDetachedFromWindow() is a method that gets called when the window has been detached from the window manager.
This is a good place to clean up any objects that contain Paint and Drawable objects that you created in
onAttachedToWindow().

#### What is onContentChanged() in Android?

onContentChanged() is a method that gets called when the content view of the screen changes. It’s often used in
activities using the Fragments API.

#### What is onCreateDialog() in Android?

onCreateDialog() is a method that gets called when a dialog is to be created. It returns an instance of Dialog.

#### What is onPrepareDialog() in Android?

onPrepareDialog() is a method that gets called every time a dialog is shown, unlike onCreateDialog() which is only
called the very first time a dialog is shown.

#### What is onSearchRequested() in Android?

onSearchRequested() is a method that gets called when the user signals the desire to start a search by pressing
the search key or invoking a search gesture.

#### What is onOptionsItemSelected() in Android?

onOptionsItemSelected() is a method that gets called whenever an item in your options menu is selected. The
default implementation simply returns false to have the normal processing happen (calling the item’s Runnable or sending
a message to its Handler as appropriate).

#### What is onOptionsMenuClosed() in Android?

onOptionsMenuClosed() is a method that gets called whenever the options menu is being closed (either by the user
canceling the menu with the back/menu button, or when an item was selected).

#### What is onPrepareOptionsMenu() in Android?

onPrepareOptionsMenu() is a method that gets called right before the menu is shown, every time it is shown. You
can use this method to efficiently enable/disable items or otherwise dynamically modify the contents.

#### What is onPostCreate() in Android?

onPostCreate() is a method that gets called after onCreate() and after the activity’s primary view has been
created. It is often used to finalize the setup of an activity, but post-creation logic here can be moved to onStart().

#### What is onPostResume() in Android?

onPostResume() is a method that gets called after onResume() and after the activity’s window’s decor view has
been marked visible. It is often used to complete the activity setup, such as starting animations.

#### What is onTitleChanged() in Android?

onTitleChanged() is a method that gets called when the activity’s title changes.

#### What is onChildTitleChanged() in Android?

onChildTitleChanged() is a method that gets called when the title of a child activity changes.

#### What is onKeyDown() in Android?

onKeyDown() is a method that gets called when a key down event has occurred. If you return true, the event is
handled and will not be passed further down the event chain.

#### What is onKeyLongPress() in Android?

onKeyLongPress() is a method that gets called when a key long press event is up. If you return true, the event
is handled and will not be passed further down the event chain.

#### What is onKeyMultiple() in Android?

onKeyMultiple() is a method that gets called when multiple key events have been fired by the system. This is a
common occurrence for keys that are auto-repeated.

#### What is onKeyUp() in Android?

onKeyUp() is a method that gets called when a key up event has occurred. If you return true, the event is handled
and will not be passed further down the event chain.

#### What is onKeyShortcut() in Android?

onKeyShortcut() is a method that gets called when a key shortcut event has occurred. If you return true, the
event is handled and will not be passed further down the event chain.

#### What is onTouchEvent() in Android?

onTouchEvent() is a method that gets called when a touch screen event has occurred. If you return true, the
event is handled and will not be passed further down the event chain.

#### What is onTrackballEvent() in Android?

onTrackballEvent() is a method that gets called when a trackball motion event has occurred. If you return true,
the event is handled and will not be passed further down the event chain.

#### What is onGenericMotionEvent() in Android?

onGenericMotionEvent() is a method that gets called when a generic motion event has occurred. If you return true,
the event is handled and will not be passed further down the event chain.

#### What is onUserInteraction() in Android?

onUserInteraction() is a method that gets called when the user interacts with the application. It’s often used
to reset user inactivity timers or to take some action when the user interacts with your application.

#### What is onWindowAttributesChanged() in Android?

onWindowAttributesChanged() is a method that gets called when the current Window of the activity has changed
attributes.

#### What is onWindowFocusChanged() in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses focus.
This is the best indicator of whether this activity is visible to the user.

#### What is onCreateThumbnail() in Android?

onCreateThumbnail() is a method that gets called when the system needs a new thumbnail for this activity’s task.

#### What is onCreateDescription() in Android?

onCreateDescription() is a method that gets called when the system needs a description of this activity’s current
state.

#### What is onProvideAssistData() in Android?

onProvideAssistData() is a method that gets called when the system needs additional information to provide
contextual help to the user.

#### What is onProvideKeyboardShortcuts() in Android?

onProvideKeyboardShortcuts() is a method that gets called when the system needs to populate the built-in help
with information about your application’s keyboard shortcuts.

#### What is onEnterAnimationComplete() in Android?

onEnterAnimationComplete() is a method that gets called when the enter animation has completed and the activity
is fully visible.

#### What is onTopResumedActivityChanged() in Android?

onTopResumedActivityChanged() is a method that gets called when the top resumed activity changes.

#### What is onVisibleBehindCanceled() in Android?

onVisibleBehindCanceled() is a method that gets called when the activity’s background visibility changes.

#### What is onActionModeFinished() in Android?

onActionModeFinished() is a method that gets called when an action mode you previously started has been
terminated.

#### What is onActionModeStarted() in Android?

onActionModeStarted() is a method that gets called when an action mode is being started for this window.

#### What is onAttachedToWindow() in Android?

onAttachedToWindow() is a method that gets called when the window has been attached to the window manager.

#### What is onDetachedFromWindow() in Android?

onDetachedFromWindow() is a method that gets called when the window has been detached from the window manager.

#### What is onWindowAttributesChanged() in Android?

onWindowAttributesChanged() is a method that gets called when the current Window of the activity has changed
attributes.

#### What is onWindowFocusChanged() in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses focus.
This is the best indicator of whether this activity is visible to the user.

#### What is onCreateThumbnail() in Android?

onCreateThumbnail() is a method that gets called when the system needs a new thumbnail for this activity’s task.

#### What is onCreateDescription() in Android?

onCreateDescription() is a method that gets called when the system needs a description of this activity’s current
state.

#### What is onProvideAssistData() in Android?

onProvideAssistData() is a method that gets called when the system needs additional information to provide
contextual help to the user.

#### What is onProvideKeyboardShortcuts() in Android?

onProvideKeyboardShortcuts() is a method that gets called when the system needs to populate the built-in help
with information about your application’s keyboard shortcuts.

#### What is onEnterAnimationComplete() in Android?

onEnterAnimationComplete() is a method that gets called when the enter animation has completed and the activity
is fully visible.

#### What is onTopResumedActivityChanged() in Android?

onTopResumedActivityChanged() is a method that gets called when the top resumed activity changes.

#### What is onVisibleBehindCanceled() in Android?

onVisibleBehindCanceled() is a method that gets called when the activity’s background visibility changes.

#### What is onActionModeFinished() in Android?

onActionModeFinished() is a method that gets called when an action mode you previously started has been
terminated.

#### What is onActionModeStarted() in Android?

onActionModeStarted() is a method that gets called when an action mode is being started for this window.

#### What is onAttachedToWindow() in Android?

onAttachedToWindow() is a method that gets called when the window has been attached to the window manager.

#### What is onDetachedFromWindow() in Android?

onDetachedFromWindow() is a method that gets called when the window has been detached from the window manager.

#### What is onWindowAttributesChanged() in Android?

onWindowAttributesChanged() is a method that gets called when the current Window of the activity has changed
attributes.

#### What is onWindowFocusChanged() in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses focus.
This is the best indicator of whether this activity is visible to the user.

#### What is onCreateThumbnail() in Android?

onCreateThumbnail() is a method that gets called when the system needs a new thumbnail for this activity’s task.

#### What is onCreateDescription() in Android?

onCreateDescription() is a method that gets called when the system needs a description of this activity’s
current state.

#### What is onProvideAssistData() in Android?

onProvideAssistData() is a method that gets called when the system needs additional information to provide
contextual help to the user.

#### What is onProvideKeyboardShortcuts() in Android?

onProvideKeyboardShortcuts() is a method that gets called when the system needs to populate the built-in help
with information about your application’s keyboard shortcuts.

#### What is onEnterAnimationComplete() in Android?

onEnterAnimationComplete() is a method that gets called when the enter animation has completed and the activity
is fully visible.

#### What is onTopResumedActivityChanged() in Android?

onTopResumedActivityChanged() is a method that gets called when the top resumed activity changes.

#### What is onVisibleBehindCanceled() in Android?

onVisibleBehindCanceled() is a method that gets called when the activity’s background visibility changes.

#### What is onActionModeFinished() in Android?

onActionModeFinished() is a method that gets called when an action mode you previously started has been
terminated.

#### What is onActionModeStarted() in Android?

onActionModeStarted() is a method that gets called when an action mode is being started for this window.

#### What is onAttachedToWindow() in Android?

onAttachedToWindow() is a method that gets called when the window has been attached to the window manager.

#### What is onDetachedFromWindow() in Android?

onDetachedFromWindow() is a method that gets called when the window has been detached from the window manager.

#### What is onWindowAttributesChanged() in Android?

onWindowAttributesChanged() is a method that gets called when the current Window of the activity has changed
attributes.

#### What is onWindowFocusChanged() in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses focus.
This is the best indicator of whether this activity is visible to the user.

#### What is onCreateThumbnail() in Android?

onCreateThumbnail() is a method that gets called when the system needs a new thumbnail for this activity’s task.

#### What is onCreateDescription() in Android?

onCreateDescription() is a method that gets called when the system needs a description of this activity’s current
state.

#### What is onProvideAssistData() in Android?

onProvideAssistData() is a method that gets called when the system needs additional information to provide
contextual help to the user.

#### What is onProvideKeyboardShortcuts() in Android?

onProvideKeyboardShortcuts() is a method that gets called when the system needs to populate the built-in help
with information about your application’s keyboard shortcuts.

#### What is onEnterAnimationComplete() in Android?

onEnterAnimationComplete() is a method that gets called when the enter animation has completed and the activity
is fully visible.

#### What is onTopResumedActivityChanged() in Android?

onTopResumedActivityChanged() is a method that gets called when the top resumed activity changes.

#### What is onVisibleBehindCanceled() in Android?

onVisibleBehindCanceled() is a method that gets called when the activity’s background visibility changes.

#### What is onActionModeFinished() in Android?

onActionModeFinished() is a method that gets called when an action mode you previously started has been
terminated.

#### What is onActionModeStarted() in Android?

onActionModeStarted() is a method that gets called when an action mode is being started for this window.

#### What is onAttachedToWindow() in Android?

onAttachedToWindow() is a method that gets called when the window has been attached to the window manager.

#### What is onDetachedFromWindow() in Android?

onDetachedFromWindow() is a method that gets called when the window has been detached from the window manager.

#### What is onWindowAttributesChanged() in Android?

onWindowAttributesChanged() is a method that gets called when the current Window of the activity has changed
attributes.

#### What is onWindowFocusChanged() in Android?

onWindowFocusChanged() is a method that gets called when the current Window of the activity gains or loses focus.
This is the best indicator of whether this activity is visible to the user.

Source: https://medium.com/@sujathamudadla1213/android-activities-interview-quetion-and-answers-880bc03efef9