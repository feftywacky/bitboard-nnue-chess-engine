# ThrawnEngine
IN DEVELOPMENT <br>
chess engine in c++ that uses a bitboard data structure and a piece square tables evaluation (nnue in the future)

## Updates
- null move pruning
- late move reduction
- iterative deepening (also adjusting aspiration window)
- principal variation search
- move history (quiet and killer)
- quiescence search
- negamax alpha beta search
- piece table evaluation
- uci compliant
- passes perft test! <3

## Features
- ~1500 ELO?
- Implements UCI protocol
- Uses bitboard data structure for fast move generation

## Compiling ThrawnEngine
currently only supports windows machines with 64-bit CPUs
### Compiler:
```bash
g++ --version
```
> g++ (x86_64-posix-seh-rev0, Built by MinGW-W64 project) 7.3.0

### Build and Run:
```bash
cd src
g++ -std=c++17 -Ofast -flto -c main.cpp engine.cpp bitboard.cpp bitboard_helpers.cpp constants.cpp fen.cpp move_helpers.cpp perft.cpp uci.cpp search.cpp evaluation.cpp
g++ -o chess main.o engine.o bitboard.o bitboard_helpers.o constants.o fen.o move_helpers.o perft.o uci.o search.o evaluation.o
chess.exe
``` 

## TODO
- time control
- improve evaluation function
- tansposition tables
- nnue

## BUGS/POTENTIAL ISSUES
- none for now 
