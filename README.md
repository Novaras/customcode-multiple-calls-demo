Small demo showing how only the last `addCustomCode` call is honoured by the game.

The Kushan Probe's `.ship` file has two calls, one to `script_a`'s `A` function, and a second to `script_b`'s `B` function. Both are on different timings.

Only `B` is called.
