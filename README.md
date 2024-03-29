# strats-ocaml
Lightweight standup calendar

This is an experiment building the same micro-app in multiple languages for a bake-off.

This app is the ocaml version. There will also be one each for [F#](https://github.com/scally/strats-fsharp)/[Rescript](https://github.com/scally/strats-rescript), which are other ML descendants. There is also a Javascript implementation in NextJS for a more familiar point of comparison.

## build

First, install ocaml. This usually requires you to install **opam**, ocaml's package manager. Further instructions are available [here.](https://dev.realworldocaml.org/install.html)

You may also need to install **dune**, a build system for ocaml. After the previous steps are complete, you just need to use opam to install it:

`opam install dune`

Once that's done, use dune to build a native executable, like so:

`dune build`

## run

`dune exec ./strats.exe`

## api

The API is located at http://localhost:3000 by default, and offers these endpoints:

`/today` view today's schedule

`/day/:day` view schedule for day N

`/schedule` view yearly schedule

`/liveness` health check

`/config` view configuration
