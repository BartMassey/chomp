## Background

Chomp is a very simple game played with a chocolate
bar. This
[Wikipedia article](https://en.wikipedia.org/wiki/Chomp)
describes the rules of the game.

Chomp is a good game to build a computer player for. Chomp
is a two-player perfect-information terminating game, so a
straightforward implementation of the Negamax algorithm can
play perfectly on small boards.

The basic idea is that in a given position a best move can
be found by exploring all possible moves, all possible
responses, etc. The resulting move selected is one that
gives the opponent the worst possible end-of-game result.

## Assignment

In this assignment, you will write a library crate that
implements a Chomp AI, and a binary crate that allows the
game to be played on the command line.

A skeleton crate has been provided at
<https://github.com/pdx-cs-rust/hw-chomp-skeleton>. Clone
this skeleton to start your project:

    git clone https://github.com/pdx-cs-rust/hw-chomp-skeleton chomp

Using the comments in the skeleton, edit `src/lib.rs` to
implement a Chomp AI, and edit `src/main.rs` to implement a
chomp game that uses the AI. Also edit `Cargo.toml` and
`README.md` to reflect your solution.

## Hints

- The `prompted` crate from `crates.io` may be useful to get
  a line of user input.

- Negamax is confusing. Use the course chat if you're lost;
  we can also put up more materials as things come up.

## Requirements

- You must edit `Cargo.toml` to provide your authorship
  information.

- You must edit `README.md` to reflect your work. Explain
  what the program and library does, and how to build and
  run the program. Comment on any issues you encountered, or
  anything else a reader might find useful.

- Both your crates must be adequately documented with
  Rustdoc comments for each datatype, function and
  method. The provided skeleton provides comments for its
  supplied functions.

- Your crates must build with current `stable` Rust.

- Your crates should contain adequate tests (implemented
    using `#[test]` unit-testing) and assertions
    (implemented using `assert!()` and related macros) for
    you to be comfortable that everything is working
    correctly.

-   Your code must be formatted according to the official Rust
    formatting style --- use `cargo fmt` to reformat your code in-place.

-   Your code must produce no compiler warnings, and `cargo clippy` must
    also produce no warnings. Please do not disable warnings except in
    the most unusual circumstances: fix them instead.

Please submit a ZIP archive containing:

-   Your `Cargo.toml` and `Cargo.lock`.

-   Your `src/lib.rs` and `src/main.rs`.

-   Any other source or other text files that are necessary/useful.

-   A `README.md` file in Markdown format giving a writeup of what you
    did, how it went, and how you tested your work.

-   Nothing else. Not your git repo. None of the funny Mac garbage
    files. Not your `target/` directory.
