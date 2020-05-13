# Convert Time Kata

Given an integer representing the number of seconds, write a function that returns a string in the following format:

>  \[a\] year(s), \[b\] day(s), \[c\] hour(s), \[d\] minute(s), \[e\] second(s) 

The terms a, b, c, d, and e represent the number of years, days, hours, minutes, and seconds respectively. Here are the rules:

* You must use the largest units of time available. You cannot, for instance, output _63 seconds_. You should instead output _1 minute, 3 seconds_.
* If there is only a single unit (i.e. 1 minute, 1 hour) the output must be listed as singular.  You should, for instance, output _1 minute_, not _1 minutes_.
* You can use the following conversion scale:
  - 1 year = 31,556,952 sec
  - 1 day = 86,400 sec
  - 1 hour = 3,600 sec
  - 1 min = 60 sec

**Examples**
```
convertTime(120) => "2 minutes"
convertTime(31740616) => "1 year, 2 days, 3 hours, 1 minute, 4 seconds"
convertTime(5400) => "1 hour, 30 minutes"
```