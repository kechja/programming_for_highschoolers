# Programming for High Schoolers
---
## 0 - Why & How To Program
* Computers are really good at doing repetitive things *fast!*
* Learn what the computer can do, and break your task down into smaller and smaller chunks that the computer understands.
* *Be patient.* **Errors are are friends.** They tell us how to fix our programs. Many professional programmers use entire systems *based on errors* until they're program is done (TDD) !!!

---
## 1- Setup
### Download a Free Editor
Get an editor (the Windows OS is not recommended long-term, but will work for the basics). Mac is preferred by many developers for reliability.
  * Mac: Atom
  * Windows: Notepad++
  
### Set up Ruby
https://online.pragmaticstudio.com/courses/ruby/steps/3  
Ruby is woking when you can type in the following with success.

```bash
> ruby --version
ruby 2.3.3p222 (2016-11-21 revision 56859) [x86_64-darwin15]
```
---
Adapted from *Learning to Program* by Chris Pine  

## 2 - Numbers
Your computer is a good calculator. Play with integers and floats.
  * Does it matter what order you put things in? (Yes! *PEMDAS*)
  * What happens when you divide by integers versus floats?
  
Challenge Programs
  * How many hours are in a week?
  * How many minutes are in a year?
  * How old are you in seconds?
  * I am 1356048000 seconds old. How old am I in years? 
 ```ruby
   puts 24 * 7                               # => 168
   puts 60 * 24 * 365                        # => 525600
   puts 60 * 60 *  24 * 365 * 43             # => 1356048000
   puts 1356048000 / ( 60 * 60 * 24 * 365 )  # => 43
 ```
 ---
 ## 3 - Strings
 Try using `puts` with `12` versus `'12'`. For now use single quotes.  We'll get to double quotes in a bit. 
 Play with `*` and `+`.
 Play with escape the escape character `\` for quotes and backslashes.  

 Challenge Programs
   * Output the result of 10 + 10
   * Output the line '10 + 10'
   * Output the line '10' + '10'
   * Ouput "Programming rocks!" 10 times.
   * Output 'You\'re the best!'
   * Output a backslash.
 ```ruby
   puts 10 + 10
   puts '10 + 10'
   puts '10' + '10'
   puts "Programming rocks! " * 10
   puts 'You\'re the best!.'
   puts '\\'
 ```
---
## 4 Variables, Assignment, & Pointers
### Basic premise / lesson:
```

   Don't Repeat Yourself 

```


Think of a really long name or sentence and type that out a few times with `puts`.  

Challenges 
  * Write a program that puts a really long name in a variable, and
    uses that variable three times (saving you a lot of work!).  Make 
    sure there's proper punctuation and spacing.
  * Write a program where one variable points to another. What happens when
   you change the first variable? Explain why.
```ruby
  name = "Franklin Blanklin Robert Harrison the Third"
  puts "Hi " + name + "."
  puts "That's a really long name, " + name + "."
  puts "We'll it was nice talking to you, " + name + "."
  #
  a = "Kevin"
  b = a
  puts a             # => "Kevin"
  puts b             # => "Kevin"
  a = "John"
  puts a             # => "John"
  puts b             # => "Kevin"
```

---
## Commandline app
Challenge:  

Google how to open programs from your command line and write a program that plays a youtube song you like and opens your email program (or other program you like) for you.
```ruby
# Here's my ruby solution.
system( "open https://www.youtube.com/watch?v=biNvjeHYGt8" )
system( "open https://gmail.com" )
```
Extra credit: Can you make the program run without typing `ruby` or `bash`?

---
## Credits
Chris Pine, *Learning to Program*  
Mike and Nicole Clark,  https://pragmaticstudio.com/  

---
## Links
Overview for all ages:  http://www.computerscienceonline.org/cs-programs-before-college/

---
## TODO: Work thru to Chris Pine book chapter 9 logic.
## TODO: Do a game project from the Ruby kids book.
