# FP7-webpage Title of Project
This is a template for using your repo's README.md as your project web page. 
I recommend you copy and paste into your README file. Delete this line and the one above it, customize everything else. Make it look good!

##Authors
* Nick Lombardi
* Joshua Semedo
* Ron

##Overview
A League of Legends statistics application written in Racket and HTML5 that interfaces with the Riot API to retrieve important information regarding a players performance that is then calculated to determine the likelyhood the player will perform poorly.

##Screenshot
![screenshot showing env diagram](http://i.imgur.com/uXrEimz.png)

##Concepts Demonstrated
* **Abstraction** is used separate the HTML5 file from the Racket Web Server & Data being passed.


##External Technology and Libraries
* Riot API - http://api.riotgames.com
* Racket Web Server Library - http://docs.racket-lang.org/web-server
* JSON Library - http://docs.racket-lang.org/json


##Favorite Lines of Code
####Nick
Each team member should identify a favorite line of code, expression, or procedure written by them, and explain what it does. Why is it your favorite? What OPL philosophy does it embody?
Remember code looks something like this:
```scheme
(map (lambda (x) (foldr compose functions)) data)
```
####Josh (another team member)
This expression reads in a regular expression and elegantly matches it against a pre-existing hashmap....
```scheme
(let* ((expr (convert-to-regexp (read-line my-in-port)))
             (matches (flatten
                       (hash-map *words*
                                 (lambda (key value)
                                   (if (regexp-match expr key) key '()))))))
  matches)
```

##Additional Remarks
Anything else you want to say in your report. Can rename or remove this section.

#How to Download and Run
Open the Racket file in DrRacket, run the file. Enter a summoner name in the box, then the necessary data will be retrieved and displayed on a web page for your viewing pleasure.

Latest Release: http://google.com

