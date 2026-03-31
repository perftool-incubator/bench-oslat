# bench-oslat
[![CI Actions Status](https://github.com/perftool-incubator/bench-oslat/workflows/crucible-ci/badge.svg)](https://github.com/perftool-incubator/bench-oslat/actions)

Scripts and configuration to run the [oslat](https://github.com/xzpeter/oslat) OS latency benchmark within the [crucible](https://github.com/perftool-incubator/crucible) performance testing framework. Measures operating system scheduling latency by running busy-loop threads and recording jitter.

## Key Files

| File | Purpose |
|------|---------|
| `rickshaw.json` | Rickshaw integration: defines client/server scripts and parameter transformations |
| `oslat-base` | Base setup shared by other scripts |
| `oslat-client` | Client-side benchmark execution |
| `oslat-server-start` / `oslat-server-stop` | Optional server lifecycle scripts |
| `oslat-get-runtime` | Runtime extraction |
| `oslat-post-process` | Post-processing: parses oslat output into crucible metrics |
| `workshop.json` | Engine image build: compiles oslat from source |
