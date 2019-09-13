## Running Your First Android Project

This lesson will walk through the process of running an application in Android Studio. If you don&#39;t have Android Studio, follow the **Installing Android Studio** guide to install it. We will show you how to start a new project from scratch in Android Studio, and how to open an existing project. By the end of this tutorial, you will know how to create an application and run it on your emulator or device.

**Android Studio Setup**

 ![](https://i.imgur.com/BmymDC4.jpg)

When you open Android Studio, this is the first thing you will see. The options on the left are past projects that you have opened. If you click one, that project will open. If you&#39;re starting from scratch, click **Start a new Android Studio project.** If you cloned a repository, click **Open an existing Android Studio project**.

If you chose **Open an existing Android Studio project,** this would be your next screen.

 ![](https://i.imgur.com/9ZVLoB3.jpg)

Navigate to the place you cloned your repository. In this case, the location is C:\Users\jpade\Documents\Projects\gitmad-contacts. Android Studio usually recognizes Android projects, so you will typically see the Android Studio logo in place of a folder icon, as is the case here.


If you choose **Create a new  Android Studio project** , this will be your next screen.

![](https://i.imgur.com/bKxPcb0.jpg)

These are different activities that you can start your project with. For now, just know that an **Activity** is a single, focused thing a user can do. If you&#39;re just starting out, we recommend selecting the **Basic Activity**. Android also runs on other devices like watches, TVs, and cars. The other tabs contain starter activities for those devices.


After you select an activity, this will be your last screen before starting development.

 ![](https://i.imgur.com/teZqwWw.jpg)

- **Name** is self explanatory.
- **Package name** is the default naming structure of folders in your project. Most projects have a package name in the form of com.yourdomain.myapplication. This is a common practice with Java projects.
- **Save location** is the directory where your project will be saved. We recommend a directory that isn&#39;t too long as errors can arise when you have a long project path.
- **Language** is the language that your first activity will be written in. From here, you can select [**Java**](https://en.wikipedia.org/wiki/Java_(programming_language)) or [**Kotlin**](https://developer.android.com/kotlin). If you have an older version of Android Studio, you may also see [**C++**](https://en.wikipedia.org/wiki/C%2B%2B). Java and Kotlin are both heavily used for Android development, and there are many pros and cons to both. If you have taken [CS 1331](https://cs1331.gitlab.io/), and you understand the concepts from that course, then you know enough Java for Android development. If you understand basic programming concepts in Kotlin, then you know enough Kotlin.
- **Minimum API level** is the minimum Android version that you want your app to support. Unfortunately fragmentation is still a thing in the Android community, so it would not make sense to target the latest version. If you target a higher version, you will have access to more features, but reach fewer customers. If you target a lower version, you will have access to fewer features, but reach more customers. We recommend setting the minimum API version to **API 21: Android 5.0 (Lollipop)**
- **androidx\* artifacts** are components of Google&#39;s new [AndroidX](https://developer.android.com/jetpack/androidx) support library. We recommend that you always keep this box checked.

After you configure your project and click the finish button you will be on your way!!

# **About Android Studio**

 ![](https://i.imgur.com/uaz5uHl.jpg)

The main window of Android Studio

Android Studio is an IDE for Android development made by Google. It&#39;s a fork of [IntelliJ](https://www.jetbrains.com/idea/) by JetBrains, so if you&#39;ve used that, PyCharm, WebStorm, or any other JetBrians IDE, the interface will be familiar to you. It has all of the bells and whistles of a modern IDE.


Ten important things to look for are:

1. Your **main project directory**. All of your code will live in the app/java folder.
2. The **res/** directory. This is where things like drawables, XML layouts, and reusable values are stored
3. **Gradle build files**. This is essentially where you define a lot of the app&#39;s settings. From SDK version (saying which versions on Android this app can run on), to libraries, the build.gradle file is crucial in making an Android app.
4. The bottom bar contains **TODOs** (which will be important later), a terminal, a menu for version control, and the **build menu**.
5. The long line of folders starting at app and ending at activities is the directory that your current open file sits in.
6. The main window where you will write code.
7. The green play button is how you will **run your apps**. The dropdown menu to the left lets you select different configurations to run.
8. The menu at the bottom right lets you change Git branches, indent size, and text encoding and it also lets you jump to a specific line and column in your code.
9. Unfortunately there is no 9 on the picture :(
10. Right above the 10, the phone icon with the robot in front is the **Virtual Device Manager**.



# **Running your first app**

Before running your first app, you must allow your app to build first. **Building** is the process of bringing all of the[.jars](https://www.geeksforgeeks.org/jar-files-java/) and other dependencies together and packaging them in a way that allows you to use them in your application. If you have taken CS 2340, you likely already know a little about this process. Android uses [Gradle](https://developer.android.com/studio/releases/gradle-plugin), though you can integrate other dependency management systems as well.

 ![](https://i.imgur.com/ySeB1OB.jpg)

While the app is building, you will see this in the bottom left hand corner

When the app is finished building, the above picture will change to this. If it&#39;s your first time building an app, it will take much longer than three minutes and forty-five seconds.

 ![](https://i.imgur.com/oh1uaPe.jpg)

Once the application is finished building,click the green play button located right above the 7 on the &quot;main window of Android Studio&quot; screenshot. After you do that, a window will appear prompting you to select a device to run your app on.


 ![](https://i.imgur.com/qhFFJPT.jpg)

The Deployment Target selection window.

The Motorola Moto G5 Plus is a physical device connected to this computer, and the Pixel 2 is an emulator. Notice the API version listed for both.

After you select your device, the app will build. If the build succeeds, and there are no other problems, you will see the app open up on your phone or emulator.

 ![](https://i.imgur.com/AqV9sHF.jpg)

If you open the Run tab in the bottom of Android Studio, you will see the verbose output from the phone while the app is running. The **launcher activity,** which opens when the app is launched, is underlined in green. The device currently running the app is underlined in orange.


Congratulations! You have just ran your first Android app!