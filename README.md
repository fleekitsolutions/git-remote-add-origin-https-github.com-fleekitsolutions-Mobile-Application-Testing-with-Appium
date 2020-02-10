History
Let’s start with a little history first, back in 2011-2014, we were using tools like Selenium web driver( using Java and C# as a programming language) and Eggplant (Black Box Tool-Language used were Sensetalk) to automate test cases of Web Applications which were to run on Windows Operating System. Everything that used to run to web browsers only were expected to have mobile applications.

Explore
We started our exploration with Appium in 2015 to see if we can automate Native apps developed in Java(Android) or Objective C(iOS) and Hybrid apps. There were other tools too like calabash, Monkey Talk and Frank, but appium holds advantages like we don’t have to modify app code/ or install any external code to our app. Overall Appium concept includes Client-Server Architecture, Session, Desired capabilities, Appium Server, Appium Client, and Appium Desktop. Because we have experience using selenium with Java, it wasn't difficult for us to understand Appium.

At Present
These days almost everyone dealing with mobile apps knows, Appium is an open-source automation framework used for testing mobile apps (Hybrid and Native) and applications run on browsers on mobile devices. There is a lot of help available online and anyone can start learning it. But before you jump to low level details it’s always better to understand how it works on a high level.

How It Works
Appium client and Appium server use JSON Wire Protocol to interact. All communication processes in the form of request and response.

The good thing is we can write our test scripts in any language (Java, Python, PHP, C#, and Javascript) and use any framework to maintain it. Appium server which is developed in node.js basically gets command executes those in mobile devices.

In order to connect with iOS and Android devices, appium needs Google UI Automator and Apple Instrumentation library.  





How Appium communicate with mobile apps
Appium needs an Instrumentation library or Google UI Automator for connection between iOS-Mac and Windows-Android. These libraries are also like a framework that helps appium to perform operations on mobile devices. These operations can be related to the device state or application state.
The process is very same as the Selenium server which understands Http requests from selenium client libraries and it caters to those requests in different ways depending upon where test cases to be executed. Each platform like iOS and Android have a different method to run a test case on the device. Appium helps here and runs test cases after listening to commands from the appium server.

Appium on Android and iOS

Appium uses the UIAutomator/XCUI framework. 
Appium client connects Appium Server and communicates through JSON wire Protocol
Appium Server works with the client on sessions and checks the desired capabilities of the client and connects with the respective framework based on iOS and Android.
iOS/Android provided framework talk to bootstrap.js which is running in a simulator/emulator/real device for performing test operations.
Bootstrap.js will help execute testing operations on devices. Once the command is executed, the client revert to the Appium server with the log details of the command executed.
