+++
title = "TSP in Go"
date = "2025-01-05T22:14:54-09:00"
#dateFormat = "2006-01-02" # This value can be configured for per-post date formatting
author = ""
authorTwitter = "" #do not include @
cover = ""
keywords = ["", ""]
description = ""
showFullContent = false
readingTime = false
hideComments = false
+++

# My Introduction to the Go language
Go has long intrigued me. When doing research on the Border Gateway Protocol I stumbled upon the creator of https://bgp.tools GitHub and he had several projects written in the language. Since this person was writing in Go, it must have some utility, I thought. Since then I had wanted to do something with the language but Inever had a good reason for it. 

After I completed my undergrad, I tried doing codecademy courses on Go. These are dreadfully boring, and since I already knew how to code, I felt like I could learn the syntax on the fly while building something I was interested in. 

I wanted to extend my research on the Traveling Salesman Problem (TSP) and thought that writing an implementation of some algorithms in Go could be fun.

# The TSP in Go -  A Learning Experience
Right off the bat, I enjoyed writing the TSP implementation of the Genetic Algorithm. I followed my C++ code I wrote and made language specific modifications.  I also looked for ways to improve the code as well. 

I found writing Go code intuitive. I really like its syntax as well as its quirks. It is clearly a language designed with intentions to be useful and make one's life easier. The auto complete program and syntax checker was forcing me to write efficient and non-redundant code. I was forced to cut any fat that existed in my C++ implementation.   

Once I finished the first complete set of GA operators, I noticed in my tests how fast the program was running. I am talking about magnitudes of 20x faster than my C++ code. While I did make some modifications for performance, the code is doing a similar amount of operations. I was and am still amazed at how fast Go code runs. I questioned C++ and its perfromance benefits, and I stumbled upon this video https://www.youtube.com/watch?v=02rh1NjJLI4&t=54s. It talks about how carefully written python can be much faster than C++. The performance difference comes down to how poorly written C++ can be combiled into garbage assembly code. I thouhgt to myself, ok there is something in this C++ code that is slowing this down a ton. And since the Go implenetation is written similarily to the C++ code, Go must be removing this garbage assembly in place of something much better.  Thus proving that Go will allow someone of mediocre skill in the language to write something that runs half-decently. As I said before, I felt forced by the language to write better code. 

All things said, I had a great experience working with Go and will continue to use the language where I can in the future. 

## Genetic Algorithm in Go for the TSP
As mentioned, I essetially converted my C++ code to Go code for the Genetic Algorithm implementation.  I won't talk too much about that here because I have several documents supporting my research on the topic here [TSP](./travelingsalesman.md). 

## Christofides Algorithm
I also tackled the Christofides algorithm in Go. See my paper on it in the Traveling Salesman Project post: [TSP](./travelingsalesman.md). 
This was also nice to write in the language as its map feature made things much easier than working with C++.

### Check out the code here: https://github.com/UnderYourSpell/tspgo

## Future Work
I intend to extend my research on the TSP further, likely using my Go implementation as opposed to my C++ implementation.