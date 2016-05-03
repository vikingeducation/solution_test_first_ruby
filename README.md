solution_tdd_ruby_rails_taste
=============================






## Overview

This project gave you a change to explore TDD and Rails. If you've never worked with RSpec or Rails this gave you a change to get familiar with them for the first time. If you have you got to review core concepts of both.


## Reviewing Your Solution

While reviewing your solutions you should be asking yourself the following questions:

### RPN Calculator

* How does your calculator resolve operator presedence unambiguously?
* What is the avantage of using a stack here? I.e. `array.pop`


### In Words 

* What is the overall method by which you converted a number into a word?


### Performance Monitor

* Is your code for benchmarking around 5-6 lines?
* What could be done to make it more compact if not?


### Jumpstart Blogger

* Does your app allow a user to login?
* Is a post created with that author as the post author?
* Does your blog allow a comma separated list of tags to be added to a post?
* Does your blog allow comments to be made on a post?
* Does your comment form allow an author to be attached to the comment?



## Key Tips and Takeaways

1. **Code until green and not more.** In a TDD workflow you generally only write as much code that is needed in order to make the test pass. If you find yourself writing more code after the tests are green, ask yourself, "What purpose does this code I'm adding serve?"


1. **Make sure your tests fail when expected.** Sometimes we find ourselves with code that produces false positives and negatives when testing. It is always a good idea to alter your code to the opposite of what is expected to ensure the test fails when it should. You'll learn more about this later, but it is good to think about as early as possible.


```ruby
# RED

def hello
  "Not Hello!" #<<<<<< !!!!!
end

require "hello"

describe "the hello function" do
  it "says hello" do
    hello.should == "Hello!"
  end
end

# GREEN

def hello
  "Hello!"
end

require "hello"

describe "the hello function" do
  it "says hello" do
    hello.should == "Hello!"
  end
end
```


## Good Student Solutions

* [Chris Scavello's `learn_ruby` Solution](https://github.com/BideoWego/learn_ruby)
* [Chris Scavello's `jumpstart_blogger` Solution](https://github.com/BideoWego/jumpstartlab-blogger)



