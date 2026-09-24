# scoop-flow

[![Tests](https://github.com/samartomar/scoop-flow/actions/workflows/ci.yml/badge.svg)](https://github.com/samartomar/scoop-flow/actions/workflows/ci.yml) [![Excavator](https://github.com/samartomar/scoop-flow/actions/workflows/excavator.yml/badge.svg)](https://github.com/samartomar/scoop-flow/actions/workflows/excavator.yml)

A [Scoop](https://scoop.sh) bucket for [Flow](https://github.com/samartomar/flow): hold a
key, talk, let go, and the words paste into the window you were working in. Speech
recognition runs on your machine; there is no API key.

```pwsh
scoop bucket add flow https://github.com/samartomar/scoop-flow
scoop install flow/flow
```

Say `flow/flow`, with the bucket in front: Scoop's main bucket has a different `flow`,
Facebook's JavaScript type checker. The command this one puts on your PATH is `flow`.

The zip is unsigned, so the first launch shows Windows SmartScreen: **More info → Run
anyway**, once. Scoop checks it against the SHA-256 that each Flow release publishes
beside its zip, and the Excavator workflow here picks up new releases every four hours.

Problems with Flow itself belong in [its issues](https://github.com/samartomar/flow/issues).
