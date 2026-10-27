# openartifact-fuzz-storage

Storage for the [ClusterFuzzLite](https://google.github.io/clusterfuzzlite/) runs of
[openartifact/openartifact](https://github.com/openartifact/openartifact). Everything here is
written by CI; do not edit by hand.

| Branch | Content | Written by |
|---|---|---|
| `main` | `corpus/<fuzzer>/`: the fuzz corpus of every target | the daily batch and prune jobs |
| `gh-pages` | `coverage/`: the latest coverage report | the daily coverage job |

Pull-request fuzzing reads the corpus and the coverage report anonymously (this repository is public),
so only the scheduled workflow needs a write credential. Details:
[docs/development](https://github.com/openartifact/openartifact/blob/main/docs/development/README.md#fuzzing).
