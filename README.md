# ktorSample-Beginner

Step-1: Install Intellij Idea for developement. Befor install Intellij please check jdk install on your system.
 Please download -: https://www.jetbrains.com/idea/download/#section=mac

Step-2: After install IDE you should need configure your IDE according to ktor, so please add ktor plugin in your Intellij IDE.

Step-3: Please go to prefrences -> plugins-> Search ktor -> and install -> restart IDE.

Step-4: Now your IDE ready for developement.

Step-5: So you can create your project two type 1: With Intellij IDE 2: https://start.ktor.io 

Step-6: After create project you see your structure look like this
    
<img width="367" alt="Screen Shot 2023-02-21 at 2 42 37 PM" src="https://user-images.githubusercontent.com/12843976/220301534-e56d809d-379b-4e0c-b150-4111dd8f0810.png">

Step-7: Before proceeding first we are know about structure and file uses.

Step-8: <h3>Project Structure Understanding</h3>
<h4>build.gradle:</h4> This is kotlin version of build gradle file.It contains the dependencies we need. If you’ve worked on Android then you must be familiar with this pattern of build gradle.

<h4>application </h4> tag sets the main class as our EngineMain class from Netty. It indicates that we’re using Netty as our main engine to create and run our server.

<h4>plugins </h4> tag indicates that this is an application, uses kotlin and serialization version 1.5.31

<h4>application.conf</h4> is the configuration file for our EngineMain which is from Netty in our case. We define the server configuration parameters in this file. The key point to note in this file is the modules we set for our application which becomes the entry point(s) for our engine to look into and set up the application from. We set the ApplicationKt.module as our main entry point.

<h4>Application.kt</h4> is the main class which our server gets the entry from.
The main function of the Application class passes the controls to EngineMain.main function so as to let Netty engine set up the rest for us.

