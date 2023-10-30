# Design Methodologies 
* Structured design
* Function oriented design
* Object oriented design


### Coupling and Cohesion
Key concepts in software engineering that are used to measure the quality of a software system's desgin. They are both important for determining scalability, reliability and maintainability of software's system.


**Coupling**- degree of interdependence between software modules. Closely connected modules are considered high coupling, where changes in one could affect others. When modules are indepenednt of eachother they have low coupling. **A good software design will have low coupling.**


**Cohesion**- degree to which elements within a module work together to fulfil one purpse. Closely related elements have high cohesion with a single purpose. Elements which are loosely related and have several purposes have low cohesion. **A good software design has high cohesion.**


### Top-Down and Bottom-Up Approaches
| Top Down      | Bottom Up   |
| -----------   | ----------- |
| Overview of the system is formulated without going into detail of the parts. Each part is then refined into more detail.|  Individual parts specified in detail, which are then linked to form larger components. |
|Theory-driven|Data-driven|
|  Used by structured programming languages   |  Used by object oriented programming lnaguages     |
|Used in debugging, module documentation| Used in testing |
|Decomposition approach|Composition approach|
|<ins>Advantages:</ins>|<ins>Advantages:</ins>|
|Can detect erros early|Easy to create and observe tests|
|Each step of refinement, parts become less complex|More suitable if defects occur at end of Programme|
|<ins>Disadvantages:</ins>|<ins>Disadvantages:</ins>|
|Slow in dynammic programming|Programme can't exist without the last module|
|Takes more memory as recursion is involved|More code is written as it's iterative|

Structured design and Function Oriented design are top-down strategies whilst Object Oriented desgin is a bottom-up approach. 
Object Oriented desgin can be carried out using UML diagrams, where as Function Oriented would use data flow diagrams.


### Four Pillars of Object Oriented Programming
|Pillar|Description|
|---|---|
|**Abstraction**|Hide the implementation details, allows for a function to be called wihtout understanding exactly what it's doing|
|**Encapsulation**|Bundles attributes and methods of an object together whilst restricting access of the data and methods from the outside (information hiding)|
|**Inheritance**|Allows similar classes to stack in a hierarchical way so that lower sub-classes can import and implement variables and methods from super classes|
|**Polymorphism**|Ability of an object to take on multiple forms. Allows a single interface to perform tasks for different types|


### Stratergy Pattern
Allows you to dynamically change the bahvior of an object by encapsulating it into different stratergies. Defines a family of algorithms, encapsulates each one and makes them interchangeable at runtime. Means the behaviour of an object can be extracted into seperate calsses so it can be swapped in and out. Improves code flexability and reusability whilst simplifying testing.

Stratergy Patterns typically use classes and objects that you'd find in object oriented programming but it can be implemented in function oriented programming although this is usually considered as a natural part of functional programming.


### Which design method to follow for an online payment system?
Object Oriented programming would allow for a stratergy pattern to be followed, which allows the behaviour of the class to be defined at runtime and so can monitor each payment. This will be beneficial as the steps in making a payment can be broken down into seperate algorithms, allowing for more flexibility as it may be beneficial to re-use certain algorithms elsewhere. This will also allow for a bottom-up approach meaning individual modules can be worked on and then composed together. This will also allow for the use of abstraction and polymorphism which will be beneficial in a payment system as we can use abstract classes or an interface.