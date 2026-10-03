# Cards — the games

The card games for [Cards](https://github.com/gazer77/cards), one file each. A game
lives entirely in its definition: the deck, the deal, the zones on the table, every
phase of play, the scoring, the words the table says, and the house rules. The engine
only plays what these files say, so a new game is a new file here — no code.

```
blackjack.json      a game definition
help/blackjack.md   its rules, as the in-game help shows them
```

The format is documented in the engine's
[docs/game-schema.md](https://github.com/gazer77/cards/blob/development/docs/game-schema.md).

## These are the originals

Every install of Cards carries the definitions it shipped with, built in. This
repository is where they come from, and the place to restore one from if a copy is ever
changed or lost: each file here is the game as released.

## Adding or changing a game

1. Fork this repository and add or edit a `.json` file (and its page in `help/`).
2. Open a pull request.
3. The checks run the engine against it: every definition must load and validate, lay
   out on a desktop and a phone, and play through to the end with computer players at
   every seat count it advertises. A game that does not finish, or names a rule the
   engine does not know, fails here rather than at someone's table.

The id is the file name (`hearts.json` is `hearts`); keep it lower-case with dashes.

## Licence

MIT — see [LICENSE](LICENSE). Contributions are accepted under the same terms. The rules
pages draw on Foster's *Complete Hoyle* (1917), which is in the public domain.
