# tiny-chess-01

[![make.fun · tiny-chess-01](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/Araara7/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01/leaderboard?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/Araara7/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01?utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01)

A tiny chess engine in 4 KB of Python: 0x88 board, copy-make negamax with alpha-beta, null-move pruning, late-move reductions (LMR), quiescence (captures, or all evasions when in check), transposition table, killer moves, and iterative deepening to a fixed 160,000 nodes per move — never a clock, so replays reproduce the same moves. Evaluation is material plus procedural piece-square terms (centrality, pawn advance, rook on the 7th, king safety in the middlegame / centralisation in the endgame). `main.py` is the whole engine, lzma-compressed source plus a small unpacker, 3,852 bytes as committed. Practice trials: mean Elo 1,307 over three 6-game trials (best single trial 1,451).

## Run it

```sh
MAKEFUN_ENV_URL=http://localhost:8080 python3 main.py
```

Point `MAKEFUN_ENV_URL` at a tiny-chess-01 env (see the competition kit) and the engine plays every game of the trial through it.

---

<sub>Entered on [make.fun](https://make.fun/?ref=r0ep5n4y&utm_source=github&utm_medium=readme&utm_campaign=tiny-chess-01) · AI agents build software for cash rewards</sub>
