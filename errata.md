# Errata

**p.9, ?2**: for "can compared", read "can be compared".
    (Thanks to Antonio Macías Ojeda, 2015-10-22.)

**p.13**: As printed, the <code>gopl.io/ch1/lissajous</code> program
is deterministic, not random.  We've added the statement below to
the downloadable program so that it prints a pseudo-random image
each time it is run. (Thanks to Randall McPherson, 2015-10-19.)

`rand.Seed(time.Now().UTC().UnixNano())`


**p.52, ?2**: for "an synonym", read "a synonym", twice.


**p.68**: the table of UTF-8 encodings is missing a bit from each first byte.
The corrected table is shown below.  (Thanks to Akshay Kumar, 2015-11-02.)
  
```
0xxxxxxx                             runes 0?127     (ASCII)
110xxxxx 10xxxxxx                    128?2047        (values <128 unused)
1110xxxx 10xxxxxx 10xxxxxx           2048?65535      (values <2048 unused)
11110xxx 10xxxxxx 10xxxxxx 10xxxxxx  65536?0x10ffff  (other values unused)
```

**p.74**: the comment in <code>gopl.io/ch3/printints</code> should say
`fmt.Sprint`, not `fmt.Sprintf`.


**p.76**: the comment `// "time.Duration 5ms0s` should have a closing double-quotation mark.


**p.79, ?4**: "When an untyped constant is
assigned to a variable, as in the first statement below, or
appears on the right-hand side of a variable declaration with an
explicit type, as in the other three statements, ..." has it backwards:
the <i>first</i>
statement is a declaration; the other three are assignments.
(Thanks to Yoshiki Shibata, 2015-11-09.)


**p.166, ?2**: for "way", read "a way".

