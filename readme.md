Hey there, welcome to CCRM! The Campus Course & Records Manager (CCRM) is a cool little console application built with Java that helps an institute keep track of its academic life. We designed it to be a one-stop-shop for managing all things students, courses, grades, and transcripts. Think of it as a command-line hub for campus administration.

This project was a fun exercise in putting a lot of modern Java SE features to work. We've used everything from solid OOP principles to robust exception handling, and even some powerful file I/O with Java's NIO.2 and Streams API.

Firing It Up! Getting CCRM up and running is easy peasy! You just need to have the

Java Development Kit (JDK) 1.8 or a newer version installed on your machine.

Once you've cloned this repository, you can simply compile and run the Main class. For a quick look at how the app works, check out the

USAGE.md file, which has a few example commands and details on the sample data files.

You'll also find some screenshots in the

screenshots/ folder that show off the application's menus and a few of its features.

A Quick Chat About Java Java's Story: From Humble Beginnings to a Global Star Java's journey began back in 1995, and it has evolved a ton since then. It started as a promising language and quickly grew. The 1998 J2SE 1.2 release, for example, brought in the Java Collections Framework, which made handling data much easier. But the real game-changers were

Java SE 5 in 2004, which introduced cool new things like generics and enums, and Java SE 8 in 2014, which brought us the power of functional programming with lambda expressions and the Streams API.

The Java Family: ME, SE, and EE Think of Java as a family with three main members, each with their own specialty.

Java ME (Micro Edition): This is the adventurous one, designed for small, embedded devices and early mobile phones. It's the go-to for situations where resources are limited.

Java SE (Standard Edition): This is the core of the family, the foundation for building desktop and general-purpose applications. If you're building a stand-alone app or working with a local server, you're probably using Java SE.

Java EE (Enterprise Edition): This is the big brother, built for large, network-heavy applications like web services and enterprise-level software. It takes everything from Java SE and adds powerful tools for handling massive, multi-tiered systems.

The Java Engine Room: JDK, JRE, and JVM Imagine you're building and driving a car.

The

JDK (Java Development Kit) is like the entire garage, filled with all the tools you need to build the car, including the blueprints (the compiler).

The JRE (Java Runtime Environment) is the finished car itself. It has the engine and all the necessary parts to drive it, but it doesn't have the tools to build another one.

The JVM (Java Virtual Machine) is the car's engine. It's the piece of machinery that actually makes the car go, interpreting the blueprints and making sure everything runs smoothly.

So, the

JDK is for developers, the JRE is for users, and the JVM is the powerhouse that runs the code.

Setting Up Your Workspace Installing Java on Windows Head over to Oracle's website and grab the latest JDK installer.

Run the installer and follow the simple on-screen instructions.

Once it's installed, you'll need to set up two environment variables: JAVA_HOME pointing to your JDK folder, and then add %JAVA_HOME%\bin to your system's Path variable.

Finally, open your Command Prompt and type

java -version to confirm everything is working perfectly. You can see a screenshot of this in our

screenshots/ folder.

Using Eclipse Download and install the "Eclipse IDE for Java Developers" package.

Open Eclipse and go to File > New > Java Project.

Give it a name, like CCRM, and set up your project to use the JDK you just installed.

Hit

Finish, and you're ready to start coding! We have screenshots of this process for you in the

screenshots/ directory.

Key Features & What's Under the Hood We built CCRM to showcase a wide range of Java features:

Student and Course Management: You can add, update, and manage both students and courses, with each object having its own unique set of fields like regNo and credits.

OOP Principles: We've made sure to hit all the big four! Our code uses

encapsulation to keep data safe with private fields and controlled access methods. We used

inheritance by creating a base Person class that both Student and Instructor extend. Our

Person class is also abstract, requiring concrete implementations in its subclasses. And we use

polymorphism to treat students and instructors as Person objects when it's convenient, making our code more flexible.

Modern Java APIs: We use the powerful Streams API to search and filter through courses and students. We also use the

Date/Time API for things like recording enrollment dates.

File Operations: The application can import data from simple text files and export it as well. We even have a backup function that creates a timestamped folder of your data using Java's

NIO.2 file system APIs.

Design Patterns: We've included a Singleton pattern for our AppConfig class to ensure there's only one configuration object. We also used a

Builder pattern to make creating new Course objects much cleaner.

Custom Exceptions: To make the application more robust, we've created our own custom exceptions, like DuplicateEnrollmentException and MaxCreditLimitExceededException.
