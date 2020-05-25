**CS 386 NAU Fall 2020**

* Software engineering is the topic.  What's that mean?  We'll discuss at length.

* Instructor: Alex Groce (SICCS/Building 90 Room 208 - alex.groce@nau.edu)

* Catalog description: "Involves applying software engineering and software architecture principles and techniques in the construction of complex computer programs in a team setting. Individualized and team writing and oral presentation tasks. Ethical issues."

* [Textbook](./textbook): "Building Secure & Reliable Systems: Best Practices for Designing, Implementing and Maintaining Systems", Heather Adkins, Betsy Beyer, Paul Blankinship, Ana Oprea, Piotr Lewandowski, and Adam Stubblefield.  It's free, see the linked directory.  This is basically a book on Google's experiences building high-reliability, highly secure, software systems, at  extreme (planetary?) scale, and with a sea of adversaries.  See [this page](https://landing.google.com/sre/resources/foundationsandprinciples/srs-book/) for a bit more on the book.  Henceforth book will be referred to as **BSRS**

**Course note:**

This is going to be a bit of an unconventional SE class, because I'm teaching it, and I have some different opinions on how to start things going with SE.

* The textbook is not a big list of terms like "agile", "architecture", "design", ... "waterfall".  I'm going to define some basic terms, early in the class: you need to know what architecture means in software in order to understand various things BSRS says.  We'll discuss them, perhaps, at some length, and you may have to write about them.

* But software is a form of literature -- code is of course written to be executed, but the compiler is going to make sure we accomplish that goal, at least to some extent.  Code is also _read by human beings_ and it fails at this goal much, much, more often.  Plenty of classes here ask you to write (modest-sized) programs; the capstone will ask for a big program.  This class is going to focus on the more common task of modifying and understanding existing code, using "software engineering and software architecture principles and techniques."  We're going to look at code.

* The book is about **the hard stuff**.  Reason being, while you don't initially set out when you learn the piano to play [Liszt's "La Campanella"](https://www.youtube.com/watch?v=MD6xMyuZls0) flawlessly.  BUT you likely will want to listen to and understand the structure of ambitious real music (not just "chopsticks") early on if you think you might ever want to be a great pianist.

* Building very large-scale user-facing systems that will face serious security challenges from highly-motivated, maybe nation-state, opponents, is a "La Campanella" level challenge for software.  Google has given us a book with lots of juicy _detail_ of how they do that. I could have gone for building mission-critical embedded code, which is my background at NASA's Jet Propulsion Laboratory, but more of you will be facing Google's issues than [NASA's](https://www.cs.princeton.edu/courses/archive/fall12/cos109/mars.rover.pdf), I imagine.

* Practically speaking, most students hit the workforce with no experience really thinking about hard security and reliability issues, and this shows in our software systems.  I'd like to make sure none of you contribute to this ongoing disaster, or at least if you do it's not _my_ fault.
