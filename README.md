# Ruby Instance Variable Modification Bug
This repository demonstrates a common misunderstanding in Ruby regarding how instance variables are accessed and modified.

The `bug.rb` file shows a class with a getter method (`value`) for an instance variable (`@value`).  Although it seems like it could be used to set a new value, in reality it only returns the current value.  Trying to assign a new value through this getter will not affect the object's state. 

The `bugSolution.rb` file provides a solution illustrating the correct way to modify instance variables.