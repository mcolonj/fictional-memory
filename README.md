# Speech Processor Framework
Nothing yet...

## Tools
Some tools associate with speech processing.


### Command line sentiment analysis through unix pipes.
1. Parse Whole Text
```
cat tools/example.txt | ./sentimentifying
```

2. Parse text by sentence
```
cat tools/example.txt | ./sentimentifying -s
```

3. Parse text by sentence and show comparative
```
cat tools/example.txt | ./sentimentifying -sc
```

4. clibboard
```
pbpaste | ./sentimentifying
```

5. Send file text to clipboard then sentimentify then to stdout. This way if your happy with your sentiment analysis you can just copy into email or textbox for sending.
```
cat example.txt | pbcopy; pbpaste | ./sentimentifying -s
```

## Options
-s parse by sentence.
-c show comparative score.

## Sample Output
```
Well totally awesome night fellas [4] Till the next great meet-up in two weeks [3] Everything was on point and excellent [3] Except when ryan abandoned the crew and fell on sidewalk wtf [-6] lol [3]  However, He is still the champion [0]
 [0]
 ````
