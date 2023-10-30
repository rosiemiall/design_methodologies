# Design Methodologies 
## Coupling and Cohesion
Key concepts in software engineering that are used to measure the quality of a software system's desgin. They are both important for determining scalability, reliability and maintainability of software's system.


**Coupling**- degree of interdependence between software modules. Closely connected modules are considered high coupling, where changes in one could affect others. When modules are indepenednt of eachother they have low coupling. **A good software design will have low coupling.**


**Cohesion**- degree to which elements within a module work together to fulfil one purpse. Closely related elements have high cohesion with a single purpose. Elements which are loosely related and have several purposes have low cohesion. **A good software design has high cohesion.**

| Top Down      | Bottom Up   |
| -----------   | ----------- |
| Overview of the system is formulated without going into detail of the parts. Each part is then refined into more detail.|  Individual parts specified in detail, which are then linked to form larger components. |
|  Used by structured programming languages   |  Used by object oriented programming lnaguages     |
|Used in debugging, module documentation| Used in testing |
|Decomposition approach|Composition approach|
|<ins>Advantages:</ins>|<ins>Advantages:</ins>|
|Can detect erros early|Easy to create and observe tests|
|Each step of refinement, parts become less complex|More suitable if defects occur at end of Programme|
|<ins>Disadvantages:</ins>|<ins>Disadvantages:</ins>|
|Slow in dynammic programming|Programme Can't exist without the last module|
|Takes more memory as recursion is involved|More code is written as it's iterative|