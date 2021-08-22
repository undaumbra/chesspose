## Description:

[Chesspose](https://undaumbra.github.io/chesspose/web/) is an experiment to play with transposition ciphers utilizing the movement of chess pieces.

Encryption works by assigning each letter of plaintext to a square on the board. After loading a game using a PGN, each move will swap two squares (where the piece came from and where it moved to).

Once the game has completed the ciphertext will be produced. Decryption is the same process, but in reverse.

The PGN acts as the key, instead of communicating a PGN directly a description of a game could be provided, ex.: "Paul Morphy vs. Duke Karl (1858)".

## Current Limitations:
- Using a game with unmoved pieces will leave parts of the plaintext unmodified
- Transposition order is not configurable (left to right, top to bottom)
- Adds space characters for padding when plaintext is not % 64
- Chesspose board is not interactive
- Implemented in JavaScript
- Uses a single game / PGN
- Only allows legal moves
