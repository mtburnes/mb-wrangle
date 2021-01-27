# mb-wrangle

## My Play
(Hamlet)[http://shakespeare.mit.edu/hamlet/full.html]

## Speaker #1
Horatio

## Speaker #2
Hamlet

## My Question
How many times did those two speakers speak?
Horatio:

`cat full.html | grep '<b>HORATIO</b>' -c`

Total of 112  times.

Hamlet:

`cat full.html | grep '<b>HAMLET</b>' -c`

Total of 359  times.
