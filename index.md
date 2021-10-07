## GrobChess API

Welcome to the documentation for the [GrobChess](https://github.com/IsaacThoman/GrobChess) API. You can use this API to create and interact with games on GrobChess.com.


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



### Support or Contact

Having trouble with Pages? Check out our [documentation](https://docs.github.com/categories/github-pages-basics/) or [contact support](https://support.github.com/contact) and we’ll help you sort it out.
