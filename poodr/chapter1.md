# Chapter 1. Object-Oriented Design

##### In object-oriented design the world is modeled as a series of messages that pass between objects.
* Failures of OOD may look like failures of code, but are actually failures of perspective.
* The first requirement for learning how to do OOD is to immerse yourself in objects, in order to acquire an OO perspective.

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
  
##### Design principles
* SOLID Acronym
  * **S**ingle Responsibility
  * **O**pen-Closed
  * **L**iskov Substitution
  * **I**nterface Segregation
  * **D**ependency Inversion
* DRY (Don't Repeat Yourself)
* LoD (Law of Demeter)

##### How design fails
* Undesigned applications are simple to write but gradually become impossible to change.
* Overdesigned applications can be resistant to change if a new feature isn't part of its design.
* OO software fails when the act of design is separated from the act of programming.
  * Design should be a progressive act of discovery that relies on a feedback loop. The iterative nature of Agile development allows design to adjust regularly and evolve naturally.
  * Software should be built in tiny increments, iterating towards an application that meets needs/requirements.

##### Procedural languages
* Procedural languages know about a small, fixed set of different kinds of data - things like `strings`, `numbers`, `arrays` etc. 
* These kinds of data are known as *data types* and are different to each other. The `string` data type is different to the `array` data type.
* Data types can be packaged into variables and your expectations about which operations you can use are based on your knowledge of a variable's data type.
* All data types and operations are built into the syntax of the language and cannot be added to.
* There is a chasm between data and behaviour.
  * Data is packaged into variables and passed to behaviour.

##### Object-oriented languages
* In Ruby, data and behaviour is combined in an *object*.
  * Objects have behaviour and may contain data.
  * Objects invoke one another's behaviour by sending each other *messages*.
* Ruby has a `string` *object* instead of a `string` *data type*. The operations (behaviour) are built into the `string` *objects* themselves instead of Ruby's syntax.
* `String` objects provide their own operations, so Ruby does not need to know anything about their data type, it only needs to provide objects a way to send messages.
  * For example, if strings understand the `concat` message, Ruby doesn't have to contain syntax to concatenate strings, it only needs to provide a way for one object to send the `concat` message to another.

##### Classes
* `Classes` provide a blueprint for the creation of similar objects.
* A class defines methods (behaviour) and attributes (variables).
* Methods are called in response to messages sent to the object.
  * The same method name can be used by different objects. Ruby's job is to find the right method of the correct object for a sent message.
* OO languages are open-ended. Just as the `string` class manufactures new string objects, the `class` class manufactures new classes.
