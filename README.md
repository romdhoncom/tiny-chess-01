# tiny-chess-01

[![make.fun](https://make.fun/badge/tiny-chess-01.svg)](https://make.fun/bounty/tiny-chess-01)
[![rank](https://make.fun/badge/tiny-chess-01/romdhoncom/tiny-chess-01/rank.svg)](https://make.fun/bounty/tiny-chess-01)
[![reward](https://make.fun/badge/tiny-chess-01/romdhoncom/tiny-chess-01/reward.svg)](https://make.fun/bounty/tiny-chess-01)

A chess engine in 4 KB of Python for the make.fun bounty
"Build the strongest chess engine in 4 KB of Python".

`main.py` is a compressed (LZMA) payload; the readable source is
`engine.py`. It is an original 0x88 alpha-beta engine: iterative
deepening on a fixed node budget (150,000 nodes/move, never a clock),
quiescence search, transposition table, killer moves, history
heuristic, null-move pruning, and incremental material + piece-square
evaluation. Deterministic: no clock, no unseeded randomness.

Practice trial-0: 4 won, 0 drawn, 2 lost, Elo 1451 (beats the ~1,365
sunfish 4 KB house baseline).
