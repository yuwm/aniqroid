# **NEW Version 3.5 [Download](http://aniqroid.sileria.com) #**



<div><a href='http://aniqroid.sileria.com'><img src='http://aniqroid.sileria.com/images/aniqroid.png' /></a></div>

Aniqroid is a toolkit that contains a collection of some very useful classes and packages that can help easing up Android development.

Android misses a very important layer of convenience API in its framework.

See details here: [API Specification](http://aniqroid.sileria.com/doc/api)

### Usage: ###

  * `Kit.init()` MUST be called before using this library. See Kit for info.
  * `Kit.destroy()` MUST be called on app termination to free all resources.

### API Higlights: ###

  * Highly optimized and top-notch LRU based Image caching/loading mechanism:
    * **A ImageCache for global caching of images in memory.
    *** A CachedImageLoader for loading image from URLs in background threaded pools, caching these images (in memory or on disk) and then either sending notification or conveniently setting them directly to provided ImageViews.


  * Rapid creation of `ListView`s and `GridView`s made easy with a very powerful class; **`AbstractListAdapter`**
  * One of the most handy class is **`ReflectiveAction`** which is similar to `EventHandler` class introduced in JDK 1.4 but more specialized towards user interation callback in Android e.g. `OnClickListener`.

It allows you to trigger a method instead of creating anonymous classes for every click and press listener in your code; Hence making it more organized in your code and more optimized for yout RAM footprint.

Please see [Java Platform Performance - Chapter 6](http://java.sun.com/docs/books/performance/1st_edition/html/JPClassLoading.fm.html#11197) for more insight in this topic.

  * Background tasks available are:
    * **`ReflectiveTask`**: Reflective version of `AsyncTask`
    * **`RemoteTask`**: Used to wrap **`RemoteRequest`** and its subclasses to perform webservice request in the worker thread
    * **`ImageLoader`** and **`QueuedImageLoader`**: for loading images from webservices in background thread
    * **`Timer`**: Similar to `java.util.Timer` but UI thread safe.

  * **`Resource`**: Easily access resources anywhere in your code without needing to have a `Context` instance handy all the time. This class provides many shortcuts and convenicence methods to access the resources programmatically.

  * Simple and easy to use location-based classes are **`SimpleLocator`** and **`Locator`** that uses LocatorListener to notify any of the first location available from GPS and NETWORK. You can also start the GPS listener first and provide a time-out to trigger NETWORK location after so many milliseconds if GPS lock is not achieved.

  * **`FramePanel`** and **`RelativePanel`** are subclasses of FrameLayout and `RelativeLayout` which provide more handy listener method to get callback for certain events and states instead of having to subclass this classes. Also available **`LinearPanel`**.

  * **`SlidingTray`** is a copy of `SlidingDrawer` but lets you create the view programmatically and allows you to put the handle on all four corners instead of just right and bottom oriented.

  * Animation classes are in com.sileria.android.anim package containing classes like `FlipAnimation`, `TransitionAnimation`, `AlphaImageAnimation` etc...

  * **`Effects`** class is an effort to collect some cool compositing and special effects APIs.

  * **`Tools`** contains methods to create Views programmatically without the need of all the boiler plate code

  * **`Utils`**, **`IO`** and **`NetUtil`** are subsets of the Commons API.

  * **`SeekBarPreference`** is one of the most wanted widget that lets you put a SeekBar into the Preference and persists the value as int. Preference activity in Android has very few widgets available at this point.


---


_Special Thanks to Jetbrains for providing us open-source license for [IntelliJ](http://www.jetbrains.com/idea/). The best IDE standing upto it's slogan: **Develop with pleasure**_.