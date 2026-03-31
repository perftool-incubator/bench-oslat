# Bench-oslat

## Purpose
Scripts and configuration to run the oslat OS latency benchmark within the crucible framework. Measures operating system scheduling latency by running busy-loop threads and recording jitter.

## Language
Bash — all scripts

## Key Files
| File | Purpose |
|------|---------|
| `rickshaw.json` | Rickshaw integration: client/server scripts, parameter transformations |
| `oslat-base` | Base setup shared by other scripts |
| `oslat-client` | Client-side benchmark execution |
| `oslat-server-start` / `oslat-server-stop` | Optional server lifecycle management |
| `oslat-get-runtime` | Extracts runtime from command-line options |
| `oslat-post-process` | Parses oslat output into crucible metrics |
| `workshop.json` | Engine image build: compiles oslat from source |

## Conventions
- Primary branch is `master`
- Standard Bash modelines and 4-space indentation
