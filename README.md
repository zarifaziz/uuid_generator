Learning MVC Architecture:
- Model is dealing with data
- View is a presentation of the model in a particular format
- The controller is the logic that binds the two

In the tutorial, there was initially one UUID class, but that was separated
into `Model`, `TkView`, and `Controller` class.

There's a few things we can do to improve this a bit more:
- Initially, the Controller class was dependent on the TkView class which is a
specific Tk implementation of the View. So, we created an Abstract class
`View(ABC)` so the Controller can be dependent on an abstract class instead.
- There was also a `Strategy Pattern` implementation in the way the UUIDs are
generated.

Architecture Level - MVC
Design Level - Functional strategy pattern
Low Level - Particular Syntax structures such as list, random.choice etc

There are other Architecture patterns such as:
- Pipeline architecture e.g. scikit-learn
- Client Server architecture 
- Peer to Peer
- Microservices e.g. big applications

[10 common software architecture patterns (link)](https://towardsdatascience.com/10-common-software-architectural-patterns-in-a-nutshell-a0b47a1e9013)
