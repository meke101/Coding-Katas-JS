# Calculate Binary Scores

Given an array of even and odd positive numbers, you need to work out if each number is odd or even.

If it is odd, you need to convert it to binary code and count how many 1's there are. If the number is even, you need to convert it to binary code and count how many are 0's there are.

You need to keep track of the odd number scores for 1s and the even number scores for 0s and after getting the final scores, you need to return which team won by either returning:

```
odds win
```
```
evens win
```
or
```
tie
```

For example with an array of [2, 3]:

`2` is even and `2` converted to binary is `10` so the score for even numbers (based on the number of `0`s in the binary) is 1.
`3` is odd and `3` converted to binary is `11` so the score for even numbers (based on the number of `1`s in the binary) is 2.

Therefore calculateBinaryScores would return `odds win`

Don't feel like you should know about binary, bits etc. This is just a soft introduction so you become aware of more features in JavaScript :)

You will need to research how to change an integer into binary. Here are some interesting/relevant articles :

  * https://developer.mozilla.org/en-US/docs/Web/JavaScript/Reference/Global_Objects/Number/toString
  * https://en.wikipedia.org/wiki/Radix
  * https://en.wikipedia.org/wiki/Binary_number


You can use these examples to start building up your test suite:

```
calculateBinaryScores([1])
  // -> 'odds win'
```

```
calculateBinaryScores([1, 2])
  // -> 'tie'
```

```
calculateBitScores([1, 2, 3, 4, 5])
  // -> 'odds win'
```

```
calculateBitScores([1, 20])
  // -> 'evens win'
```
