# Welpher's Homebrew Tap

A personal [Homebrew](https://brew.sh) tap for my macOS apps and command-line tools.

## Install

Tap once:

```bash
brew tap welpher/tap
```

Then install any package by name:

```bash
brew install --cask lantransport   # GUI app
# brew install <formula>           # command-line tool
```

You can also install directly without tapping first:

```bash
brew install --cask welpher/tap/lantransport
```

## Casks

| Package | Description |
| --- | --- |
| [`lantransport`](Casks/lantransport.rb) | Share files across your local network |

## Formulae

Nothing here yet. Command-line tools will live in `Formula/`.

## Notes

- Cask builds are universal macOS binaries (Apple Silicon + Intel) unless stated otherwise.
- Some apps are not notarized yet, so macOS may ask you to confirm the first launch
  (right-click → Open).
- Source code for each package lives in its own repository; this tap only contains
  the Homebrew metadata.

## Adding a package

- Casks go in `Casks/<name>.rb`
- Formulae go in `Formula/<name>.rb`

Each project's release automation should update only its own file, so that
concurrent updates from different projects don't collide.
