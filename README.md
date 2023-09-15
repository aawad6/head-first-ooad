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

Having a lot of Strings? That’s terrible... try use enums or objects instead which will lead to less fragile application along the way. That means less problems for the customer, and less maintenance for us.

**Test drive** - After getting the right requirements from the customer now we need to make sure we’ve actually got those requirements handled by our code. so we need to test things out, and see if our app is working like customer wants it to.

Use a textual description of the problem you’re trying to solve to make sure that your design lines up with the intended functionality of your application.

**Objectville world** - when objects are very particular about their jobs. Each object is interested in doing its job, and only its job, to the best of its ability. 
> There’s nothing a well-designed object hates more than being used to do something that really isn’t its true purpose.

**Encapsulation** allows you to hide the inner workings of your application’s parts, but yet make it clear what each part does.
> Anytime you see duplicate code, look for a place to encapsulate!

**Delegation** - when an object needs to perform a certain task, and instead of doing that task directly, it asks another object to handle the task (or sometimes just a part of the task).
> Delegation lets each object worry about equality (or some other task) on its own. This means your objects are more independent of each other, or more loosely coupled.

**Loosely coupled** - when each object have a specific job to do, and it does only that job. So the functionality of your app is spread out over lots of well-defined objects, which each do a single task really well.

All this time that we’ve been talking about the three steps you can follow to write great software, we’ve really been talking about OOA&D.  
OOA&D is really just an approach to writing software that focuses on making sure your code does what it’s supposed to, and that it’s well designed. That means your code is flexible, it’s easy to make changes to it, and it’s maintainable and reusable.

### BULLET POINTS
* It takes very little for something to go wrong with an application that is fragile.
* You can use OO principles like encapsulation and delegation to build applications that are flexible.
* Encapsulation is breaking your application into logical parts that have a clear boundary that allows an object to hide its data and methods from other object.
* Delegation is giving another object the responsibility of handling a particular task.
* Always begin a project by figuring out what the customer wants.
* Once you've got the basic functionality of an app in place work on refining the design so it's flexible.
* With a functional and flexible design, you can employ design patterns to improve your design further and make your app easier to reuse.
* Find the parts of your application that change often, and try and separate them from parts of your application that don't change.
* Building an application that works well but is poorly designed satisfies the customer but will leave you with plain, suffering, and lots of late nights fixing problems.
* Object oriented analysis and design (OOA&D) provides a way to produce well-designed applications that satisfy both the customer and the programmer.

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
It's a list of steps that describes what your system does to accomplish a particular customer goal. Use case usually have a **main path** and **alternate paths**.
> Use cases are all about the “what.” Don’t worry about the “how” in this stage.

#### One use case, three parts
- Clear Value: A single use case focuses on a single goal. 
- Start and Stop: Something must begin the process, and then there must be a condition that indicates that the process is complete.
- External Initiator: Sometimes that initiator is a person, but it could be anything outside of the system. (The user (or users) are outside of the system, not a part of it.)

Remember to checking your requirements against your use cases.
> You need to go back to your requirements and make sure that they’ll cover everything your system has to do. And that’s where the use case comes in.

### BULLET POINTS
* **Requirements** are things your system must do to work correctly.
* Your initial requirements usually come from your customer.
* To make sure you have a good requirements, you should develop use cases for your system.
* **Use Cases** details exactly what your system should do.
* A use case has a **single goal**, but can have multiple paths to reach that goal.
* A good use case has a **starting** and **stopping condition,** an **external initiator**, and **clear value** to the user.
* A use case is a simply a story about how your system works.
* You will have at least one use case for each goal that your system must accomplish.
* After your use cases are complete, you can refine and add to your requirements.
* A requirements list that makes all your use cases possible is a good set of requirements.
* Your system must work in the real world, not just when everything goes as you expect it to.
* When things go wrong, your system must have **alternate paths** to reach the system's goals.
