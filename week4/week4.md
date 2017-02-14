Interactive Journalism - Advanced Data & Coding module
========================================================

Module code: JOM299

A gentle introduction to R

Housekeeping
========================================================

## Presentations:
Either Wed 22nd or Fri 24th February

http://doodle.com/poll/hbizsz6kqedvgsd4

**Fill it in, please!**

Reminder
========================================================

> Pick one journalism piece/tool that illustrates a format or technique. Produce a presentation and report on the piece, how it's built, and the landscape of that format/technique in online journalism today.

Example topics
========================================================

Some examples (please don't use these - come up with one of your own!):

https://www.nytimes.com/interactive/2017/01/15/us/politics/you-draw-obama-legacy.html  
Storytelling interactivity

https://www.buzzfeed.com/heidiblake/the-tennis-racket  
Algorithmic journalism, computer-assisted journalism

https://www.theguardian.com/world/interactive/2013/nov/01/snowden-nsa-files-surveillance-revelations-decoded  
All-rounder


More example topics
========================================================

https://panamapapers.icij.org/  
http://panamapapers.sueddeutsche.de/articles/56febff0a1bb8d3c3495adf4/  
Relational database, network analysis, follow-the-money approach

http://drones.pitchinteractive.com/  
Data-led storytelling

http://www.jplusplus.org/en/project/rentswatch/  
Crowdfunding + scraping

http://newsroom.tools/  
http://soundcite.knightlab.com/  
http://otranscribe.com/  
Journalism Tools

This week: intro to R
========================================================

An overview of R: http://www.nature.com/news/programming-tools-adventures-with-r-1.16609


Tool of choice (on university computers, or free download): **RStudio**

RStudio is an IDE:

* A text editor
* An interpreter to run your script or commands
* And many other tools

Variables
========================================================

```
> a = 1
> print(a)
1
```

or

```
> a <- 1
> print(a)
1
```

Operations like we expect them:

```
> a <- 3
> b <- a*a
> print(b)
9
```

A list = a "vector"
========================================================

In Python world, we'd write

```
list = [1, 2, 10]
```

In R, however, lists are called *vectors*

```
list <- c(1, 2, 10)
```

We have indexes... but not zero-padded like in Python

```
> list[1]
1
> list[3]
10
```

Instant operations on vectors:

```
> list +2
3 4 12
```

Some awesome with vectors
========================================================

```
list <- c(1, 2, 10)
```

Mean of values in list:

```
> mean(list)
4.33333
```

Exponential:

```
> exp(list)
2.718282  7.389056  22026.465795
```

Confusion: the data frame
========================================================

http://www.r-tutor.com/r-introduction/data-frame

> A data frame is a list of vectors of equal lengths

```
> list <- c(1, 2, 10)
> names <- c("one", "two", "ten")
> qualifications <- c("simple", "double", "rubbish")
> df <- data.frame(list, names, qualifications)

> print(df)

  list   names     qualifications
1    1   one         simple
2    2   two         double
3   10   ten        rubbish
```

More data frame madness
========================================================

```
> print(df)

  list   names     qualifications
1    1   one         simple
2    2   two         double
3   10   ten        rubbish

> print(df[2])
  names
1   one
2   two
3   ten
```

Shorthands
========================================================

You can use `$` and the column name to access the list items

```
> print(df)

  list   names     qualifications
1    1   one         simple
2    2   two         double
3   10   ten        rubbish

> df$names
one  ten  two
```

Good bit: you can create/edit columns with way

```
> df$names <- "lol"  #rename all items in column
> df$example <- True # add new column
> print(df)
  list names qualifications example
1    1   lol         simple    True
2    2   lol         double    True
3   10   lol        rubbish    True
```

Operations on data frames
========================================================

Canonical way:

Create a new data frame as the result of an operation on the previous

Why? We keep versions in memory and can have a look at if things worked well

```
new_dataframe <- old_dataframe + 1
```

More example topics
========================================================

More example topics
========================================================

More example topics
========================================================

More example topics
========================================================

More example topics
========================================================


