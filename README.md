# ExJack
JACK interface for Elixir using Rustler-based NIF.

The purpose of this library is to provide an audio outlet for Elixir through all platforms. However, if you're on Linux, and don't need JACK outright, it's probably preferable to use [ExAlsa](https://github.com/FraihaAV/ex_alsa) and interface with ALSA directly.

## Requirements
```
Tested with:
JACK 2 (see https://github.com/RustAudio/rust-jack)
Elixir 1.12
Rust 1.56.1
```

## Set-up (OSX)
```
brew install jack
brew services start jack

mix test
```

It may help to view what's going with JACK using a GUI like https://qjackctl.sourceforge.io/.

## TODO
- [x] Play audio frames 
- [ ] Documentation (generate ExDoc + usage with additional examples)
- [ ] Input access
- [ ] Additional tests/typespecs in Rust/Elixir
- [ ] Release initial version to Hex
