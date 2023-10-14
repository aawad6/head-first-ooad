_This is my summary of Head First Object Oriented Analysis and Design._

_If you are the publisher and think this repository should not be public, just write me an email at ammaryasser085 [at] gmail [dot] com and I will make it private._

**Contributions:** Issues, comments, and pull requests are super welcome.

# Head First Object Oriented Analysis and Design

Book by Bertt D. Mclaughlin, Gary Pollice, and David West.

- [Chapter 1: Well-Designed Apps Rock](#chapter-1-well-designed-apps-rock)
- [Chapter 2: Gathering Requirements](#chapter-2-gathering-requirements)
- [Chapter 3: Requirements Change](#chapter-3-requirements-change)
- [Chapter 4: Analysis](#chapter-4-analysis)
- [Chapter 5: Part 1: Good Design](#chapter-5-part-1-good-design)
- [Chapter 5: Part 2: Flexible Software](#chapter-5-part-2-flexible-software)
- [Chapter 6: Solving Really Big Problems](#chapter-6-solving-really-big-problems)
- [Chapter 7: Architecture](#chapter-7-architecture)
- [Chapter 8: Design Principles](#chapter-8-design-principles)
- [Chapter 9: Iteration and Testing](#chapter-9-iteration-and-testing)
- [Chapter 10: The OOA&D Lifecycle](#chapter-10-the-ooa&d-lifecycle)

## Chapter 1: Well-Designed Apps Rock
How do you really write great software? It’s never easy trying to figure out where to start. Does the application actually do what it’s supposed to? And what about things like duplicate code—that can’t be good, can it? It’s usually pretty hard to know what you should work on first, and still make sure you don’t screw everything else up in the process.

Great software in 3 easy steps:
1. Make sure your software does what the customer wants it to do.
2. Apply basic OO principles to add flexibility.
3. Strive for a maintainable, reusable design.

Having a lot of Strings? That’s terrible... try to use enums or objects instead which will lead to less fragile application along the way. That means less problems for the customer and less maintenance for us.

**Test drive** - After getting the right requirements from the customer now we need to make sure we’ve actually got those requirements handled by our code. so we need to test things out and see if our app is working like the customer wants it to.

Use a textual description of the problem you’re trying to solve to make sure that your design lines up with the intended functionality of your application.

**Objectville world** - when objects are very particular about their jobs. Each object is interested in doing its job, and only its job, to the best of its ability. 
> There’s nothing a well-designed object hates more than being used to do something that really isn’t its true purpose.

**Encapsulation** allows you to hide the inner workings of your application’s parts, yet make it clear what each part does.
> Anytime you see duplicate code, look for a place to encapsulate it!

**Delegation** - when an object needs to perform a certain task, and instead of doing that task directly, it asks another object to handle the task (or sometimes just a part of the task).
> Delegation lets each object worry about equality (or some other task) on its own. This means your objects are more independent of each other, or more loosely coupled.

**Loosely coupled** - when each object has a specific job to do, and it does only that job. So the functionality of your app is spread out over lots of well-defined objects, which each do a single task really well.

All this time that we’ve been talking about the three steps you can follow to write great software, we’ve really been talking about OOA&D.  
OOA&D is really just an approach to writing software that focuses on making sure your code does what it’s supposed to, and that it’s well designed. That means your code is flexible, it’s easy to make changes to it, and it’s maintainable and reusable.

### BULLET POINTS
* It takes very little for something to go wrong with an application that is fragile.
* You can use OO principles like encapsulation and delegation to build applications that are flexible.
* Encapsulation is breaking your application into logical parts that have a clear boundary that allows an object to hide its data and methods from other objects.
* Delegation is giving another object the responsibility of handling a particular task.
* Always begin a project by figuring out what the customer wants.
* Once you've got the basic functionality of an app in place work on refining the design so it's flexible.
* With a functional and flexible design, you can employ design patterns to improve your design further and make your app easier to reuse.
* Find the parts of your application that change often, and try to separate them from parts of your application that don't change.
* Building an application that works well but is poorly designed satisfies the customer but will leave you with plain, suffering, and lots of late nights fixing problems.
* Object-oriented analysis and design (OOA&D) provides a way to produce well-designed applications that satisfy both the customer and the programmer.

## Chapter 2: Gathering Requirements
Everybody loves a satisfied customer. You already know that the first step in writing great software is making sure it does what the customer wants it to. But how do you figure out what a customer really wants?

**Requirement** - It’s a specific thing your system has to do to work correctly.
> When it comes to requirements, the best thing you can do is let the customer talk. And pay attention to what the system needs to do; you can figure out how the system will do those things later.

### Steps of Gathering The Requirements
- Listen to the customer.
- Creating a requirements list.
- Plan for things going wrong.
- Update your list of things.

### Use Case
It's a list of steps that describes what your system does to accomplish a particular customer goal. Use cases usually have a **main path** and **alternate paths**.
> Use cases are all about the “what.” Don’t worry about the “how” at this stage.

#### One use case, three parts
- Clear Value: A single use case focuses on a single goal. 
- Start and Stop: Something must begin the process, and then there must be a condition that indicates that the process is complete.
- External Initiator: Sometimes that initiator is a person, but it could be anything outside of the system. (The user (or users) are outside of the system, not a part of it.)

Remember to check your requirements against your use cases.
> You need to go back to your requirements and make sure that they’ll cover everything your system has to do. And that’s where the use case comes in.

### BULLET POINTS
* **Requirements** are things your system must do to work correctly.
* Your initial requirements usually come from your customer.
* To make sure you have good requirements, you should develop use cases for your system.
* **Use Cases** details exactly what your system should do.
* A use case has a **single goal**, but can have multiple paths to reach that goal.
* A good use case has a **starting** and **stopping condition,** an **external initiator**, and **clear value** to the user.
* A use case is simply a story about how your system works.
* You will have at least one use case for each goal that your system must accomplish.
* After your use cases are complete, you can refine and add to your requirements.
* A requirements list that makes all your use cases possible is a good set of requirements.
* Your system must work in the real world, not just when everything goes as you expect it to.
* When things go wrong, your system must have **alternate paths** to reach the system's goals.

## Chapter 3: Requirements Change
In the real world, requirements are always changing, and it’s up to you to roll with these changes and keep your customer satisfied.

Change is constant, and your system should always improve every time you work on it.

Requirements always change. If you’ve got good use cases, though, you can usually change your software quickly to adjust to those new requirements.
> Sometimes a change in requirements reveals problems with your system that you didn’t even know were there.

Alternate path - It's one or more steps that a use case has that are optional, or provide alternate ways to work through the use case.

scenario - A complete path through a use case, from the first step to the last.
> Most use cases have several different scenarios, but they always share the same user goal.

### BULLET POINTS
* Requirements will always **change** as a project progresses.
* When requirements change, your system has to evolve to handle the new requirements.
* When your system needs to work in a new or different way, begin by updating your use case.
* A **scenario** is a single path through a use case, from start to finish.
* A single use case can have multiple scenarios, as long as each scenario has the same customer goal.
* **Alternate paths** can be steps that occur only some of the time, or provide completely different paths through parts of a use case.
* If a step is optional in how a system works, or a step provides an alternate path through a system, use numbered sub-steps.
* You should almost always try to **avoid duplicate code**. It's a maintenance nightmare and usually points to problems in how you've designed your system.

## Chapter 4: Analysis
Your application has to do more than work on your own personal development machine, finely tuned and perfectly set up; your apps have to work when real people use them.

Analysis helps you ensure your system works in a real-world context.

Textual analysis - Looking at the nouns (and verbs) in your use case to figure out classes and methods.
> Pay attention to the nouns in your use case; in a use case, the nouns are usually the classes you need to write and focus on in your system.

### From good analysis to good classes:
- A good use case clearly and accurately explains what a system does, in language that’s easily understood.
- With a good use case complete, textual analysis is a quick and easy way to figure out the classes in your system.

### UML Terms
Class diagrams are great for modeling the classes you need to create, but they don’t provide all the answers you’ll need in programming your system.

````java
allowedBarks: Bark[*]
````
[*] indicates the **multiplicity** of an attribute: how many of a certain type the attribute can hold.

The asterisk '\*' indicates that *allowedBarks* can hold an unlimited number of *Bark* objects.

Association - a solid line from one class to another is called an association. It means that one class is associated with another class by reference, extension, inheritance, etc.

Remember, in Chapter 1, we said that delegation helps our applications stay loosely coupled. That means that your objects are independent of each other; in other words, changes to one object don’t require you to make a bunch of changes to other objects.
> Delegation shields your objects from implementation changes to other objects in your software.

### BULLET POINTS
* Analysis helps you ensure that your software works in the real-world context, and not just in a perfect environment.
* Use cases are meant to be understood by you, your managers, your customers, and other programmers.
* You should write your use cases in whatever format makes them most usable to you and the other people who are looking at them.
* A good use case precisely lays out what a system does, but does not indicate how the system accomplishes the task.
* Each use case should focus on only one customer goal. If you have multiple goals, you will need to write multiple use cases.
* Class diagrams give you an easy way to show your system and its code constructs at a 10,000-foot view.
* The attributes in class diagrams usually map to the member variables of your class.
* The operations in class diagrams usually represent the method of your classes.
* Class diagrams leave lots of details out, such as class constructors, some type of information, and the purpose of operations in your classes.
* Textual analysis helps you translate a use case into code-level classes, attributes, and operations.
* The nouns of a use case are candidates for classes in your system, and the verbs are candidates for methods in your system's classes.
* **Delegations** shields your object from implementation changes to other objects in your software.

## Chapter 5: Part 1: Good Design
Change is inevitable. No matter how much you like your software right now, it’s probably going to change tomorrow. And the harder you make it for your software to change, the more difficult it’s going to be to respond to your customer’s changing needs.

Abstract classes - placeholders for actual implementation classes. They define behavior, and the subclasses implement that behavior.
> Whenever you find common behavior in two or more places, look to abstract that behavior into a class, and then reuse that behavior in the common classes.

One of the best ways to see if the software is well-designed is to try and **CHANGE** it.

### OO Principles:
- Coding to an interface, rather than to an implementation, makes your software easier to extend.
> By coding to an interface, your code will work with all of the interface’s subclasses—even ones that haven’t been created yet.

- Encapsulation is more than just avoiding lots of copy-and-paste, it helps you protect your classes from unnecessary changes.

- Each class should have only one reason to change.
> When you see a class that has more than one reason to change, it is probably trying to do too many things. See if you can break up the functionality into multiple classes, where each individual class does only one thing—and therefore has only one reason to change.

### UML Terms (again)
Interface - the interface in UML has the "<<interface>>" word and italicized *class name*.

Abstract class - *the name of a class* is in italics. Here, we don’t want anyone creating instances of that class; it’s just used to provide a common base for specific implementation classes.

Aggregation "A line with a diamond ---<>" - a special form of association, and means that one thing is made up (in part) of another thing. 

A line with an arrow that isn’t colored in means generalization. You use a generalization to show that a class extends and inherits behavior from a more generalized class.

## Chapter 5: Part 2: Flexible Software
When you run into problems making changes to your application, it probably means that your software needs to be more flexible and resilient.

**Code once, look twice (or more!)**. Keep looking over your designs when you run into problems. A decision you made earlier may be what’s causing you headaches now.

**Pride kills good design**. Never be afraid to examine your own design decisions, and improve on them, even if it means backtracking.

By encapsulating what varies, you make your application more flexible, and easier to change.

When you have a set of properties that vary across your objects, use a collection, like a Map, to store those properties dynamically.

Most good designs come from analysis of bad designs, so never be afraid to make mistakes and then change things around.

Cohesion - A cohesive class does one thing well and does not try to do or be something else.
> Cohesion is just a measure of how closely related the functionality of the classes in an application are. If one class is made up of functionality that’s all related, then it has only one reason to change.

The **more cohesive** your software is, the **looser the coupling** between classes. 

Great software is usually about being **good enough**.
> Spending hours trying to write “perfect software” is a waste of time; spending lots of time writing great software and then moving on, is sure to win you more work, big promotions, and loads of cash and accolades.

## Chapter 6: Solving Really Big Problems
You’ve got a ton of tools in your OOA&D toolbox, but how do you use those tools when you have to build something really big?

The best way to solve a big problem is by breaking it into lots of functional pieces, and then working on each of those pieces individually.

Commonality - One way you can find out more about a system is to figure out what the system is like.

Variability - Another great way to find out what a system should do is to figure out what it’s not like.

Feature - a high-level description of something a system needs to do. A single feature results in multiple different requirements.
> Get features from the customer, and then figure out the requirements you need to implement those features.

### Use Case Diagram
After figuring out the system requirements you might think of writing use cases, but **use cases don’t always help you see the big picture**. A use case diagram could be just what you need.
> Use case diagrams are the blueprints for your system.

Use your feature list to make sure your use case diagram is complete.

Domain analysis - The process of checking your designs, and describing a problem using terms the customer will understand.

Design pattern - It's a way to design the solution for a particular type of problem. i.e. Model View Controller pattern.

### How To Solve Big Problems
1. Listen to the customer, and figure out what they want you to build.
2. Put together a feature list, in a language the customer understands.
3. Make sure your features are what the customer actually wants. (domain analysis)
4. Create blueprints of the system using use case diagrams (and use cases).
5. Break the big system up into lots of smaller sections.
6. Apply design patterns to the smaller sections of the system.
7. Use basic OOA&D principles to design and code each smaller section.

### BULLET POINTS
* The best way to look at a big problem is to view it as a collection of smaller problems.
* Just like in small projects, start working on big projects by gathering features and requirements.
* Features are usually 'big' things that a system does, but also can be used interchangeably with the term "requirements".
* Commonality and variability give you points of comparison between a new system and things you already know about.
* Use cases are detail-oriented; use case diagrams are focused more on the big picture.
* Your use case diagram should account for all the features in your system. 
* Domain analysis is representing a system in language that the customer will understand.
* An actor is anything that interacts with your system but isn't part of the system.

## Chapter 7: Architecture
It’s time to take all those little pieces laying around your workspace, and figure out how to turn them into a well-ordered, well-designed application.

Architecture - your design structure, and highlights the most important parts of your app, and the relationships between those parts.

The things in your application that are really important are architecturally significant, and you should focus on them FIRST, when you’re trying to figure out if something is architecturally significant, there are three questions you can ask:
- Is it part of the essence of the system?
> Can you imagine the system without that feature? If not, then you’ve probably found a feature that is part of the essence of a system.
- What the heck does it mean?
> Anytime you’re unsure about what something is, it could create problems with the rest of the system. Spend time on these features early, rather than late.
- How the heck do I do it?
> If you have no idea how you’re going to tackle a particular problem, you better spend some time upfront looking at that feature, so it doesn’t create lots of problems down the road.

Focus on one feature at a time to **reduce risk** in your project, and don’t get distracted by features that won’t help reduce risk.

In this stage (architecture) we’re focusing on doing just the things that reduce risk, no matter what are these things, it could be writing a code for a couple of classes or even drawing a class diagram for others. 
> Sometimes the best way to write great code is to hold off on writing code as long as you can.

Architecture is all about reducing the risks of you delivering your software late, or having it not work like the customer wants it to. Our key feature list, class diagrams, and those partially done classes all help make sure we’re not just developing great *code*, but that we’re developing great *software*.

If at any time you're unsure about what a feature means and how you need to implement that feature in your system:
1- Ask the customer.
2- Apply Commonality analysis.
3- Put an implementation plan.

### BULLET POINTS
* Architecture helps you turn all your diagrams, plans, and feature lists into a well-ordered application.
* The features in your system that are most important to the project are architecturally significant.
* Focus on features that are the essence of your system, that you’re unsure about the meaning of, or unclear about how to implement first.
* Everything you do in the architectural stages of a project should reduce the risks of your project failing.
* If you don't need all the details of a use case, writing a scenario detailing how your software could be used can help you gather requirements quickly.
* When you're not sure what a feature is, you should ask the customer, and then try and generalize the answers you get into a good understanding of the feature.
* Use commonality analysis to build software solutions that are flexible.
* Customers are a lot more interested in software that does what they want, and comes in on time, than they are in code that you think is really cool.
