# GoLang Cheat Sheet 

I learn faster if I take the time to write things down, and I am getting old and find that if I create a reference for my self I am just being kind to the future me.  

I also believe if I find this information useful I think others will too.

This is my GoLang Reference.  Things I find usefull, Things I need to remember and resources I use.


## Learning

### TODO
I put the this section at the top so I never forget it.

#### What I need to read about but did not have time

- [Golang channels](http://guzalexander.com/2013/12/06/golang-channels-tutorial.html)
- [Goroutines, Closures, and You](https://blog.opsee.com/goroutines-closures-and-you-60aadcf285ba#.sgh39up7g)
- [Stopping Goroutines](https://medium.com/@matryer/stopping-goroutines-golang-1bf28799c1cb#.a2nvlmg0u)
- [Don't Get Bitten by Pointer vs Non-Pointer Method Receivers in Golang](https://nathanleclaire.com/blog/2014/08/09/dont-get-bitten-by-pointer-vs-non-pointer-method-receivers-in-golang/)


### Books

This is my reading list. 

- You should always start with the free book [An Introduction To Go](http://www.golang-book.com/books/intro).  It seems silly but you never know what you dont know and I found a few gems in that book I might have missed later on.

- Here is my [amazon reading list](https://www.amazon.com/gp/registry/wishlist/HGQRISNNSBRH/ref=cm_wl_list_o_5?):  I will review each book below as I read them.

### Blogs

- [Effective Go](https://golang.org/doc/effective_go.html) 
- This [video](https://www.youtube.com/watch?v=ndmB0bj7eyw) is really good in showing how you can do testing.
- I like Go by example it is a really nice resource. It pointed me to this [how to use interfaces in go](http://jordanorelli.com/post/32665860244/how-to-use-interfaces-in-go).

### Interfaces

The go interface can be extreamly cool and confusing at the same time!  


Read these:

- [Go by example, Interfaces](https://gobyexample.com/interfaces)
- [How to use interfaces in go](http://jordanorelli.com/post/32665860244/how-to-use-interfaces-in-go)
- [video](https://www.youtube.com/watch?v=ndmB0bj7eyw) on testing and how to use Interfaces to make that eaiser. 

### JSON

JSON in go is fun and exciting!  Just use structs whereever you can and only marshal json to a unknown struct if you really have to!

Read these blogs:

- [JSON and Go](https://blog.golang.org/json-and-go) Really good read.
- [JSON by example](https://gobyexample.com/json) Becaue I love this site!
- [JSON package docs](https://golang.org/pkg/encoding/json/) The examples really helped me.
- [Encode/Decode arbitrary JSON](http://michaelheap.com/golang-encodedecode-arbitrary-json/)

This tool ([json-to-go](https://mholt.github.io/json-to-go/)) is awesome for converting JSON to a struct. I love code generators!

When you have a complex json object that has a struct in a struct. brake them out and include one in the other.  This will allow more flexibility.   Here is an [example](https://play.golang.org/p/hdwgvKpeQw) on how you can do that.   I took the raw JSON and fed it through [json-to-go](https://mholt.github.io/json-to-go/) then broke the structs out and even added a method to the top struct. 


### Time

The [Time](https://golang.org/pkg/time/) package in go is quite nice.  Here are some resources around it:

- [Time formatting and parsing](https://gobyexample.com/time-formatting-parsing)

Play with it [here](https://play.golang.org/p/DCPFKZ7hER)



## SDLC

Coding in the Enterprise has some verry defined patterns.  When ever I learn a new language I am looking for how it fits in to these patterns. 

### IDE

- On my mac I like a rich editor that shows folders and files.  So I use [Sublime Text 3](https://www.sublimetext.com/3) with the [GoSublime](https://github.com/DisposaBoy/GoSublime) plugin.  

- VIM with [vim-go](https://github.com/fatih/vim-go)  I want to get [neocomplete](https://github.com/Shougo/neocomplete.vim) working but have not yet. 


### Style

- [Local scoped (private) Variables](http://www.golang-book.com/books/intro/4#section1) should be mixedCase or bumpyCaps.  This is for Variables or Constants in the private scope.


### Smell

- The [Go Vet](https://golang.org/cmd/vet/) tool will analize your code to find code that copiles but smells bad. 