# Justify Line

In this kata you should complete the function `justifyLine` that takes a string of text and returns it justified according to the maximum line length which is provided as an argument.

If the string contains more characters than the maximum line length then your function should return `"String exceeds maximum line length."`

Space between words should be padded with additional spaces so that the final word in a line touches the edge of the line. When distributing additional spaces, larger gaps should come at the start of the line (see examples)


## Examples

In this example the max line length is 16 characters. The original string has 15 characters we just add one additional space between the first two words.

```javascript
const str = 'foo foo foo foo';

justifyLine(str, 16);
--> 'foo  foo foo foo'

```

In this example the max line length is 18 characters. The original string has 15 characters so the additional 3 characters are distributed between each word.

```javascript
const str = 'foo foo foo foo';

justifyLine(str, 18);
--> 'foo  foo  foo  foo'

```


In this example the max line length is 20 characters. The original string has 15 characters so there are 5 more spaces that we need to use to pad the words. Larger gaps should go first, so 2 additional spaces are inserted in the first 2 gaps, and the final gap has 1 additional space.

```javascript
const str = 'foo  foo  foo  foo';

justifyLine(str, 20);
--> 'foo   foo   foo  foo'

```