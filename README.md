# Advanced-.NET-demos
What you will learn in this course

The goal of the Advanced .NET is to introduce developers to areas of .NET that are complex or often cause confusion. We deepen your skills in areas such as multithreading and parallel programming, crash dump capture and analysis and building easily extensible applications. We also lift the lid off of complex pieces of infrastructure like the thread pool and the garbage collector


You'll get answers to these questions:

How do I use the latest APIs to create efficient multi-threaded code?
What are the best practices for parallelizing algorithms?
How do Code Contracts help me improve code quality?
How does the Garbage Collector really work?
What are my options for building pluggable applications
How can I debug application crashes in production?
Come and learn to build robust .NET applications!

Course highlights

In this course, you learn to:

Write code that works well with the garbage collector
Use the latest threading library: PFx
Build code that can scale across multiple cores
Build pluggable and testable and applications using MEF and Inversion of Control
Improve memory usage through proper understanding of assemblies, types, and JIT compilation
Debug difficult problems using WinDBG, SOS, and ADPLUS
Course outline and topics

Day 1

PFx: Task - A Unified Threading API

When the Parallel Framework Extensions (PFx) were first announced it looked as though it was going to target a narrow set of requirements around parallelizing processor intensive code. Over time the scope of the library has grown significantly such that it will become the main model for building asynchronous code. The pivotal type enabling this transition is the Task class. This is a functionally very rich type allowing the creation of both short and long lived asynchronous work, Tasks can have dependencies on one another and support cancellation. In this, the first of the PFx modules we look specifically how this class gives us a unified framework for building multithreaded code.


Thread Safety
Asynchronous programming requires careful attention to detail since most objects are not designed with multithreaded access in mind. This module introduces the importance of Interlocked and Monitor-based synchronization.


PFx: Synchronization Primitives and Concurrent Data Structures
Ever since its inception .NET has had support for a number of synchronization primitives (such as Interlocked, Monitor and Mutex). However, on their own these primitives do not provide support for more complex synchronization situations and so people have had to use them as building blocks to build things like efficient Semaphores. PFx finally brings to the library a set of richer primitives such as lazy initialization, a lightweight semaphore and a countdown event. But more than this, it also introduces a set of high performance concurrent data structures that allow you to use them without you having to provide your own synchronization logic around them. This module looks at this new set of tools in your synchronization toolbox.

Day 2
PFx: Parallel
The initial goal of PFx was to simplify the parallelization of processor intensive tasks - and this remains a key feature. This part of its functionality is focused on the Parallel class and it's For and ForEach members. In this module we look at the simplified model but also highlight that parallelizing algorithms is never as simple as it might first seem - we show you some of the pitfalls that you should be aware of when trying to parallelize functionality using the Parallel class.


Reactive Framework
Reactive Framework is a new library that uses the .NET 4.0 IObservable interface and LINQ to create a compelling new programming model that allows you to build "event" based code with declarative LINQ statements. This module introduces the Reactive Framework and shows how it can greatly simplify your code.


Inside the Garbage Collector
The garbage collector has been part of .NET since its inception. However, exactly how the GC works is often shrouded in mystery. Also the fact that memory management is automated doesn't release the developer from caring about memory issues - it's just those memory issues appear in a different guise. In this module we take the lid of the GC, look at how it works and is optimized and then assess what this means for you when you are writing your code: things you do that can help the GC and things that cause it problems.


Day 3
Debugging with Visual Studio - beyond the basics
Visual Studio is the primary development tool for .NET developers. It includes a very rich debugging environment of which often developers have only scratched the surface. This module looks at some of the more advanced tools that are built into visual studio for debugging.


Advanced Debugging - Tooling
Some kinds of bugs require tools beyond visual studio to track down. In this module we look at other tools that you can use to, for example, capture and analyze crash dumps, profile your code generally gain deeper insight into what's really going on in that buggy application.


Advanced Debugging - Techniques
Now we have seen some of the more advanced tools at our disposal we can look at how they can be used to diagnose complex problems like multithreaded and memory related bugs. This module shows different techniques for solving common complex debugging issues.


Day 4
Getting started with Test Driven Development
Using unit testing comprehensively within software development is a growing movement. Unit testing allows refactoring and maintenance with the confidence that existing functionality is not broken. In this module we will look at techniques for writing good unit tests and integrating them into testing frameworks to automate the unit tests. We will see that using the tests to drive the development guides you to produce flexible, loosely-coupled code with high test coverage.


Designing code for testing
Code is not inherently testable; it must be designed that way. In this module we look at common issues in code that make it hard to test and how we resolve them. Along the way we will look at Dependency Injection and Inversion of Control containers.


Using Test Doubles to isolate code
Loosely coupling is essential to being able to isolate the code under test - it allows us to provide alternate versions of, say, the data access layer. However, building alternate versions to cover every test scenario would be a significant overhead. Fortunately mocking frameworks come to our rescue, allowing us to create the test conditions "on-the-fly". In this module we look at how various types of test doubles (fakes, spies, stubs and mocks) can be used to isolate the code unit and how a mocking framework helps automate a lot of this work.

