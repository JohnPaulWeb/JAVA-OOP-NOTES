# JAVA-OOP-NOTES

JAVA OOP NOTES

An Introduction to Object

Orientated Programming

Introduction
This chapter will discuss different programming paradigms and the advantages of the Object Oriented
approach to software development and modelling. The concepts on which object orientation depend
(abstraction, encapsulation, inheritance and polymorphism) will be explained.
Objectives
By the end of this chapter you will be able to...
• Explain what Object Oriented Programming is,
• Describe the benefits of the Object Oriented programming approach and
• Understand and the basic concepts of abstraction, encapsulation, generalisation and
polymorphism on which object oriented programming relies.
All of these issues will be explored in much more detail in later chapters of this book.
This chapter consists of six sections:-
1) A Brief History of Computing
2) Different Programming Paradigms
3) Why use the Object Oriented Paradigm
4) Object Oriented Principles
5) What Exactly is Object Oriented Programming?
6) The Benefits of the Object Oriented Programming Approach.
1.1 A Brief History of Computing
Computing is a constantly changing our world and our environment. In the 1960s large machines called
mainframes were created to manage large volumes of data (numbers) efficiently. Bank account and payroll
programs changed the way organisations worked and made parts of these organisations much more efficient.
In the 1980s personal computers became common and changed the way many individuals worked. People
started to own their own computers and many used word processors and spreadsheets applications (to
write letters and to manage home accounts). In the 1990s email became common and the world wide web
was born. These technologies revolutionised communications allowing individuals to publish information
that could easily be accessed on a global scale. The ramifications of these new technologies are still not
fully understood as society is adapting to opportunities of internet commerce, new social networking
technologies (twitter, facebook, myspace, online gaming etc) and the challenges of internet related crime.


The Object Oriented paradigm builds upon and extends the ideas behind the structured programming
paradigm of the 1970s.

1.3 Why use the Object Orientation Paradigm?
While we can focus our attention on the actual program code we are writing, whatever development
methodology is adopted, it is not the creation of the code that is generally the source of most problems.
Most problems arise from:-
• poor analysis and design: the computer system we create doesn’t do the right thing.
• poor maintainability: the system is hard to understand and revise when, as is inevitable,
requests for change arise.
Statistics show 70% of the cost of software is not incurred during its initial development phase but is
incurred during subsequent years as the software is amended to meet the ever changing needs of the
organisation for which it was developed. For this reason it is essential that software engineers to everything
possible to ensure that software is easy to maintain during the years after its initial creation.

The Object Oriented programming paradigm aims to help overcome these problems by helping with the
analysis and design tasks during the initial software development phase (see chapter 6 for more details
on this) and by ensuring software is robust and maintainable (see chapters 9–11 for information on the
support Object Orientation and Java provides).
1.4 Object Oriented Principles
Abstraction and encapsulation are fundamental principles that underlie the Object Oriented approach to
software development. Abstraction allows us to consider complex ideas while ignoring irrelevant detail
that would confuse us. Encapsulation allows us to focus on what something does without considering
the complexities of how it works.
Activity 3
Consider your home and imagine you were going to swap your home for a week with a
new friend.
Write down three essential things you would tell them about your home and that you would
want to know about their home.
Now list three irrelevant details that you would not tell your friend.

The Benefits of the Object Oriented Programming Approach
Whether or not you develop programs in an object oriented way, before you write the software you must
first develop a model of what that software must be able to do and how it should work. Object oriented
modelling is based on the ideas of abstraction, encapsulation, inheritance and polymorphism.
The general proponents of the object oriented approach claims that this model provides:
• better abstractions (modelling information and behaviour together)
• better maintainability (more comprehensible, less fragile)
• better reusability (classes as encapsulated components)
We will return to look at these claims later in Chapter 11 as we see a case study showing in detail how
object oriented analysis works and how the resultant models can be implemented in an object oriented
programming language (i.e. Java).
1.7 Summary
Object oriented programming involves the creation of classes by modelling the real world. This allows
more specialised classes to be created that inherit the behaviour of the generalised classes. Polymorphic
behaviour means that systems can be changed, as business needs change, by adding new specialised
classes and these classes can be accessed by the rest of the system without any regard to their specialised
behaviour and without changing other parts of the current system.

The Unified Modelling
Language (UML)
Introduction
This chapter will introduce you to the roles of the Unified Modelling Language (UML) and explain the
purpose of four of the most common diagrams (class diagrams, object diagrams, sequence diagrams
and package diagrams). Particular emphasis will be placed on class diagrams as these are the most used
part of the UML notation.
Objectives
By the end of this chapter you will be able to...
• Explain what UML is and explain the role of four of the most common diagrams,
• Draw class diagrams, object diagrams, sequence diagrams and package diagrams.
The material covered in this chapter will be expanded on throughout later chapters of the book and the
skills developed here will be used in later exercises (particularly regarding class diagrams.
This chapter consists of six sections:-
1) An introduction to UML
2) UML Class Diagrams
3) UML Syntax
4) UML Package Diagrams
5) UML Object diagrams
6) UML Sequence Diagrams
2.1 An Introduction to UML
The Unified Modelling Language, UML, is sometimes described as though it was a methodology. It is not!
A methodology is a system of processes in order to achieve a particular outcome e.g. an organised
sequence of activities in order to gather user requirements. UML on the other hand a precise diagramming
notation that will allow program designs to be represented and discussed. As it is graphical in nature it
becomes easy to visualise, understand and discuss the information presented in the diagram. However
as the diagrams represent technical information they must be precise and clear – in order for them to
work therefore there is a precise notation that must be followed.

As UML is not a methodology it is left to the user to follow whatever processes they deem appropriate
in order to generate the designs described by the diagrams. UML does not constrain this – it merely
allows those designs to be expressed in an easy to use, but precise, graphical notation.
2.2 UML Class diagrams
Classes are the basic components of any object oriented software system and UML class diagrams provide
an easy way to represent these. As well as showing individual classes, in detail, class diagrams show
multiple classes and how they are related to each other. Thus a class diagram shows the architecture of
a system.
A class consists of:-
• a unique name (conventionally starting with an uppercase letter)
• a list of attributes (int, double, boolean, String etc)
• a list of methods

This is shown in a simple box structure...

ClassName
attributes

methods()

For attributes and methods visibility modifiers are shown (+ for public access, – for private access).
Attributes normally being kept private and methods normally made public.
Note: String shown above is not a primitive data type but is itself a class. Hence it starts with a capital letter.
Thus a class Book, with String attributes of title and author, and the following methods setTitle(),
getTitle(), setAuthor(), getAuthor() and toString() would be shown as...

Book
- title :String
- author :String
+setTitle()
+getTitle()
+setAuthor()
+getAuthor()
+toString()

Activity 1
Draw a diagram to represent a class called ‘BankAccount’ with the attribute balance (of type int)
and methods depositMoney() and withdrawMoney(). Show appropriate visibility modifiers.

Feedback 1

BankAccount
- balance :int
+depositMoney()
+withdrawMoney()
+displayBalance()

The diagram above shows this information
UML allows us to suppress any information we do not wish to highlight in our diagrams – this allows
us to suppress irrelevant detail and bring to the readers attention just the information we wish to focus
on. Therefore the following are all valid class diagrams...
Firstly with the access modifiers not shown...

BankAccount
balance :int
depositMoney()
withdrawMoney()
displayBalance()

Secondly with the access modifiers and the data type not shown...

BankAccount
balance :int
depositMoney()
withdrawMoney()
displayBalance()





