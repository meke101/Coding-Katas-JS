## Connect Four

Practice your Object Oriented skills to create a [Connect Four](https://en.wikipedia.org/wiki/Connect_Four) Class. The function `ConnectFourGame` should be called with the `new` keyword to return a new instance of a connect 4 game. A game should keep track of its state and should have a `play` method to allow a user to play. 

Connect Four is a connection game in which the players first choose a color and then take turns dropping colored discs from the top into a seven-column, six-row vertically suspended grid. The pieces fall straight down, occupying the next available space within the column. A player wins when they are the first to form a horizontal, vertical, or diagonal line of four of their own discs.

## Methods Required

The `getBoard` method should return the state of the board at any given time. It should be initialized as a 7 * 6 matrix filled with `null` values.

The `getPlayer` method should return a string indicating who the current player is. Use 'x' and 'o' to keep track of the players. 'x' should go first.

The `play` method should take a column index number and should drop a counter into the correct column. If the column is full it should reuturn `'This column is full'`. The function does not return anything but the new state of the board can be checked by calling `getBoard` and the next player can be checked by calling `getPlayer`.

The `checkWinner` function should check for a winner in the instance of the connectFourGame and should return `false` for no winner and should return the winner if there are 4 connected counters in either horizontal, vertical or diagonal directions.

You may find it useful to bring in functions from other katas as helpers.

## Example Functionality

```javascript
const game = new ConnectFourGame();

game.getBoard();
/*  -->
 [
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null]
  ]
  */
```

```javascript
const game = new ConnectFourGame();

game.getPlayer();
//  --> 'x'
```


```javascript
const game = new ConnectFourGame();

game.play(3);

game.getBoard();
/*
  --> [
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, 'x', null, null, null]
  ]
*/

game.getPlayer();
//  --> 'o'
```

```javascript
const game = new ConnectFourGame();

game.play(3);
game.play(2);
game.play(3);
game.play(1);
game.play(3);
game.play(0);
game.play(3);

game.getBoard();
/*
  --> [
    [null, null, null, null, null, null, null],
    [null, null, null, null, null, null, null],
    [null, null, null, 'x', null, null, null],
    [null, null, null, 'x', null, null, null],
    [null, null, null, 'x', null, null, null],
    ['o', 'o', 'o', 'x', null, null, null]
  ]
*/

game.checkWinner();
// --> 'x'

```