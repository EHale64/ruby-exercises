The `strings.rb` file has a number of exercises to help you better work with strings in ruby.  

Below is a list of methods that will help you complete the exercises - research each of them on the [Ruby Docs for Strings](https://ruby-doc.org/core-2.6.5/String.html) to learn more about what they do and how they are used.

There are additional methods that you will need to complete the exercises; each of these additional methods can be found in the Ruby Docs for Strings.

* `String#capitalize`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-capitalize)
* `String#concat`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-concat)
* `String#chomp`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-chomp)
* `String#chop`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-chop)
* `String#delete`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-delete)
* `String#include?`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-include-3F)
* `String#length`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-length)
* `String#reverse`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-reverse)
* `String#sub`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-sub)
* `String#strip`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-strip)
* `String#upcase`[docs](https://ruby-doc.org/core-2.6.5/String.html#method-i-upcase)

Here's a [companion piece to working through these exercises](https://josh.works/turing-backend-prep-02-first-tests-and-making-them-pass).

An alumn has put together [a video walkthrough](https://www.youtube.com/watch?v=BKqo2w0W7S0) for this `strings.rb` test, as well. 

These two resources, combined, should help get you up and running. 

Finally, you'll be getting your first introduction to `Minitest` in this file!

#### What is minitest?

When you cloned this repo and ran `bundle` you installed the `minitest`.  

Many of the `.rb` files in this repo begin with calling `minitest`, like:

```ruby
require 'minitest/autorun'
require 'minitest/pride'
require 'pry'

class StringTest < Minitest::Test
```
So what is minitest and what's going on above? Great question! 

See the references to minitest at the top of the file? `minitest/autorun` and `minitest/pride`?

These are “modules” of the `minitest` gem.

I strongly recommend “pausing” this exercises and reading (and re-reading, and write all the code from all the examples in) this excellent guide: [https://launchschool.com/blog/assert-yourself-an-introduction-to-minitest](https://launchschool.com/blog/assert-yourself-an-introduction-to-minitest)

I’ll state that again. Read and study the Minitest guide. It is fantastic and will set you up for success for the rest of Turing:

[https://launchschool.com/blog/assert-yourself-an-introduction-to-minitest](https://launchschool.com/blog/assert-yourself-an-introduction-to-minitest)

[...]

Did you read the Launch School post? Great! Then most of what is in this file should look a lot more readable to you.

As a quick test, answer the following questions:

- What is minitest?

   minitest is a testing framework which comes with every standard Ruby distribution. It provides assertion and expectation based interfaces 
   
- what is a Domain-Specific Language (DSL)?

  Domain-Specific Language is a computer language specific to a particular application domain. 
  
  Each one is unique and must be learned for it's specific application.
  
- What does assert_equal mean? How many arguments does it expect?

  assert_equal means that you are comparing two values and expecrting that they will be equivalent in the test you are running.
  
  It expects two arguments, one for each value.
  
- Will assert_equal true, "true" pass?
- How do you “run” a test file?

  Test files are run using the commaned line.
  
- is a “failing” test a bad thing?

  Not necessarily. Failing a test simply means that the assertion you made in the test was not true. This means that the code being tested is running correctly but that it is not producing the desired/expected outcome.
  
- does minitest run all the tests in order?

  Not unless you explicity set it up to do so.
  
- Find a list of minitest assertions (google it!). What’s a cool one you found?

Awesome. If you can answer all of those questions, you’ve got your head wrapped around Minitest. Onward!
