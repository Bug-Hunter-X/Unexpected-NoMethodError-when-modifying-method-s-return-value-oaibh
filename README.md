# Ruby Method Modification Bug

This repository demonstrates a common unexpected error in Ruby: attempting to assign a value directly to a method's return value, which often leads to a `NoMethodError`.  The `bug.rb` file shows the problematic code. The solution (`bugSolution.rb`) illustrates the correct way to modify the object's internal state. 

## How to reproduce
1. Clone this repository.
2. Run `ruby bug.rb`
3. Observe the `NoMethodError`.

## Solution
The correct approach is to either define a setter method (`value=`) or to modify the internal state (`@value`) directly through the existing methods if appropriate. The `bugSolution.rb` file demonstrates this.