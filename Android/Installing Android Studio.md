# Lesson 1.1: Installing Android Studio

This lesson will talk about installing Android Studio and configuring it so that you&#39;re ready to run your first application. It will also explain how to set up a physical device or emulator for development. By the end of this tutorial, you will have Android Studio installed, and you will be ready to run an application on your device (virtual or physical).

**Installing Android Studio**

**Requirements:**

-  [Java Development Kit](https://www.oracle.com/technetwork/java/javase/downloads/jdk8-downloads-2133151.html) (JDK) and **not** the JRE. If you&#39;ve taken a Java class, you already have this.
  - To verify, run "javac -version" in any command line application (Command Prompt, PowerShell, macOS Terminal, Git Bash, Linux Terminal, etc.)
  - You should get an output similar to "javac 1.8.0\_192", and if you don&#39;t, follow this short guide to install the JDK. [Win](https://docs.oracle.com/en/java/javase/12/install/installation-jdk-microsoft-windows-platforms.html#GUID-96EB3876-8C7A-4A25-9F3A-A2983FEC016A), [Mac](https://docs.oracle.com/en/java/javase/12/install/installation-jdk-macos.html#GUID-2FE451B0-9572-4E38-A1A5-568B77B146DE), [Linux](https://docs.oracle.com/en/java/javase/12/install/installation-jdk-macos.html#GUID-2FE451B0-9572-4E38-A1A5-568B77B146DE).
  - **Note** : You may also need to set the PATH variable. This is covered in the linked guides above.
-  You only need one of the two options below.
   1. Hardware virtualization must be enabled in your BIOS for emulators
      - This is usually enabled by default on macOS. If you have Windows, you can check if it&#39;s enabled by opening task manager, and navigating to your CPU menu under the performance tab, like [this](https://www.shaileshjha.com/wp-content/uploads/2017/02/windows_10_task_manager_performance_tab_virtualization_enabled.jpg) picture.
   2. A physical Android device with USB cord and developer mode enabled
      - To enable developer mode, navigate to your phone&#39;s build number. On most phones, this would be in Settings -\> About Phone -\> Build number. If you have an HTC, Samsung, LG, or Motorola phone, it will be in a slightly different place. (Google it)
      - Tap the build number seven times. After a few taps, you will see steps counting down until you unlock developer options.
      - After that, you will see a "_Developer options_" menu in your settings (Location will be different for different phones)



To install Android Studio, follow [this](https://developer.android.com/studio/install) guide for every OS from Google. This guide primarily consists of downloading the program.
