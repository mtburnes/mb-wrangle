# mb-wrangle

## My Play
[Hamlet](http://shakespeare.mit.edu/hamlet/full.html)

## Speaker #1
Horatio

## Speaker #2
Hamlet

## My Question
How many times did those two speakers speak?

I could have chosen to do the long command using `tr` and `sort`, but I thought there may have been an easier way.
If you use `grep '[string]'` you can attach -c to count each occurance. I found out that functionality by using `grep --help`
and it gave me exactly what I was looking for. 

Every time a character speeks in the play, the HTML looks like <b>[CHARACTER-NAME]</b>. This is a pattern throughout the whole page.
Using the `grep` commands below, I could get exactly how many times the string occured in the .html file.

Horatio:

`cat full.html | grep '<b>HORATIO</b>' -c`

Total of 112  times.

Hamlet:

`cat full.html | grep '<b>HAMLET</b>' -c`

Total of 359  times.

Grand total of 471 times.
