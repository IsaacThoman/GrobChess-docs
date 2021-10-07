## GrobChess API

Welcome to the documentation for the [GrobChess](https://github.com/IsaacThoman/GrobChess) API. You can use this API to create and interact with games on GrobChess.com.

The API is hosted at api.grobchess.com


### Getting board state
#### Returns the current state of the board

Arguments:`channel`

Example: GET `api/chess?channel=1234`

Returns:
```
"w43256234111111110000000000000000000000000000000077777777a98bc89aSTOP0000"
```

The first character is either 'w' for white's move, or 'b' for black's move. 

Chars 1-64 each represent a square on the board. The last 4 chars include the last move made in standard move notation.

### Making moves
#### Allows you to send a move to a board using standard move notation

Arguments:`message`,`channel`

Example: POST `api/chess?message=e2e4&channel=1234`

Returns:
```
200 OK
```

Checks the given move for legality and makes it on the given board number.
