# Tamarin Prover Homebrew tap

This is a [Homebrew](https://brew.sh/) [tap](https://docs.brew.sh/Taps) for the [Tamarin prover](https://tamarin-prover.github.io).

## Installing

Install Homebrew and run

```
brew install tamarin-prover/tap/tamarin-prover
```

## Building bottles
Homebrew formulae can include compiled binaries, which it calls "bottles". To build a new bottle (perhaps for a new operating system or Tamarin release):

1. `brew install --build-bottle tamarin-prover/tap/tamarin-prover`
1. `brew bottle tamarin-prover` and note the line of output it gives you with the bottle SHA and tag
1. Give the resulting file (e.g. `tamarin-prover-1.2.3.tar.gz`) to Katriel and ask him to upload it to Bintray
1. Update the `tamarin-prover` formula with the bottle SHA and tag, in the bottle section with the custom Bintray URL

New installs will then use this bottle.
