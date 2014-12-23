#### Chapter 2. Designing Classes with a Single Responsibility

###### The foundation of an object-oriented system is the *message*, but the most visible organizational structure is the *class*. 
* The goal should be to model code using classes such that it does what it is supposed to do *right* now and is also easy to change *later*.
* This involves identifying the qualities that make a class easy to change.

*Easy to change* is defined as
* Changes have no unexpected side effects
* Small changes in requirements require correspondingly small changes in code
* Existing code is easy to reuse
* The easiest way to make a change is to add code that is in itself easy to change

Code you write should have the following qualities. It should be
***Transparent** Consequences of change should be obvious in the code and in any code that relies on it.
***Reasonable** Cost of change should be proportional to the benefits
***Usable** Code should be reusable in new contexts
***Exemplary** The code itself should encourage those who change it to perpetuate these qualities

###### Classes should have a single responsibility
*A class should do the smallest possible useful thing.
