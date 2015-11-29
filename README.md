# earley-parser
My implementation of the [Earley parser](https://en.wikipedia.org/wiki/Earley_parser) for syntactic parsing of sentences according to a context-free grammar (CFG). (Implemented for Question #3 of Assignment #2, COMP 599, McGill University.)

### Usage

Example usage:

```
python earleyparser.py sample-grammar.txt < sample-sentence.txt
```

More generally, you can run the parser as follow,

```
python earleyparser.py <grammer_file>
```

which reads sentences from standard in, one at a time, printing the parses to standard output using pretty_print(), with parses separated by an extra newline. For sentences that do not have a parse according to the grammar, it prints the sentence back out, unchanged.

Running with the `draw` option, like so,

```
python earleyparser.py draw <grammer_file>
```

displays the parses using NLTK's tree-drawing.

See `sample-grammar.txt` on how to format your grammar. (The parser program requires each rule to only produce non-terminal or terminal symbols, not both.)

### License

MIT
