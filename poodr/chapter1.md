# Chapter 1. Object-Oriented Design

##### In object-oriented design the world is modeled as a series of messages that pass between objects.
* Failures of OOD may look like failures of code, but are actually failures of perspective.
* The first requirement for learning how to do OOD it to immerse yourself in objects in order to acquire an OO perspective.

##### Good design anticipates change
* Change is inevitable. At the initial point of design, perfect knowledge of future requirements is not possible.
* Applications that are easy to change are flexible, adaptable, and pleasurable to code.

##### Why change is hard
* OO applications are made up of parts which interact to produce the behaviour of the whole.
  * The parts are *objects*. Interactions are *messages* that pass between these parts.
  * The sender of a message must know things about the receiver. This creates dependencies.
* OOD is about *managing dependencies*
  * Objects that know too much about each other can wreak havoc when change occurs.
  * When objects know too much they have many expectations, which need to be fulfilled for them to work. These expectations mean small changes can have large effects.
  
##### Design Principles
* SOLID Acronym
  * **S**ingle Responsibility
  * **O**pen-Closed
  * **L**iskov Substitution
  * **I**nterface Segregation
  * **D**ependency Inversion
* DRY (Don't Repeat Yourself)
* LoD (Law of Demeter)
