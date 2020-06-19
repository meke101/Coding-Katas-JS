## Simplify Directions

The challenge is to implement a function that takes an array of directions and simplifies them. Directions can be simplified if any two directions cause the person to end up in the same place. For example, the directions `["NORTH", "SOUTH"]` cancel one another out and the function should return an empty array of no directions `[]`

##### More Examples

Here are some examples to help you build out your test suite:

```javascript
simplifyDirections(["NORTH", "SOUTH", "WEST"])
    --> ["WEST"]
```


```javascript
simplifyDirections(["NORTH", "WEST", "SOUTH", "WEST", "EAST"])
    --> ["WEST"]
```


```javascript
simplifyDirections(["NORTH", "EAST", "SOUTH", "WEST", "NORTH", "NORTH"])
    --> ["NORTH", "NORTH"]
```
