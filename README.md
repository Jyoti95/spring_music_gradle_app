# spring_music_gradle_app

for this gradle app steps are:
1).first install gradle binary file from this link:http://bryanlor.com/blog/gradle-tutorial-how-install-gradle-windows
2). set the environment variables as from above link.
3).then use commandas
gradle clean assemble
cf push
Difficulty - Beginners
It'll be a piece of cake.  This cake is no lie.

Prerequisites
Windows 8 (or any Windows version)
Java JDK installed
Instructions
Download Gradle at their site: http://www.gradle.org/downloads .
Unzip the package to anywhere you want to keep it.  I normally put these kinds of things in my development directory where other goodies go into also.
Now, right click on "Computer" (a.k.a. "My Computer") and then select "Properties":
gradle-tutorial-1.png

Then click on "Advance system settings":
gradle-tutorial-2.png

Now, you should already be on the "Advanced" tab, so click on "Environment Variables...":
gradle-tutorial-3.png

Then we want to add a new user variable for us called JAVA_HOME.  Click on "New..." as shown below:
gradle-tutorial-4.png

Now enter JAVA_HOME into the input field for "Variable name:":  
gradle-tutorial-5.png

For "Variable value:", we want to enter the location of your Java JDK directory.  The Java JDK on my computer is located in it's default installation location, C:\Program Files\Java\jdk1.8.0_25:  
gradle-tutorial-6.png

When finished, click "OK".
Under "System variables", look for the "Variable" called Path
gradle-tutorial-7-new.png

Now we want to add additional paths to our PATH environment variable, so let's click on "Edit..." under "System variables" as shown below:
gradle-tutorial-8.png

Then proceed to the end of the value and enter the \bin locations of both Gradle and the Java JDK.  
gradle-tutorial-9.png

For Gradle, I entered it as C:\gradle-2.1\bin .  For the Java JDK, enter only %JAVA_HOME%\bin because %JAVA_HOME% will use the user variable we defined earlier to get your Java JDK directory for you.
gradle-tutorial-10.png

 After you're done entering the new bin paths for Gradle and the Java JDK, click "OK".  Click "OK" a couple more times to back out.
Now, let's test it out.  Open up command prompt and type gradle -v and you should see something similar:
