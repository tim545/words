
Words
=====

Generates lists of random **single syllable** words, good for placeholder values or id's. The idea was inspired from http://what3words.com

The list of words came from http://research.haifa.ac.il/~nancyh/wordlist.html

###### Usage

Download, include into your webpage with a `<script>` tag and create a new `Words` object with `new Words(options)`. The `options` parameter is an object which can have any of these properties:

```
{
    n: 3, // Number of words to return
    delimiter: '.' // A string to separate the words, defaults to a space
}
```

###### Methods

`word()` simply returns a singe random word.

`words()` returns multiple words defined by the options.



```
var w = new Words({
    n: 3,
    delimiter: '.'
});

var placeholder = w.words(); // "draft.toy.more"

```

###### To do

- multi language
- return array instead of string with an option
- return only words which have a word length falling within a range
- return only words which has a certain first vowel, e.g. 'a'
