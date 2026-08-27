# Bench-oslat

## Purpose
Scripts and configuration to run the oslat OS latency benchmark within the crucible framework. Measures operating system scheduling latency by running busy-loop threads and recording jitter.

## Language
- Bash for client/server execution scripts
- Python for post-processing (`oslat-post-process.py`)

## Key Files
| File | Purpose |
|------|---------|
| `rickshaw.json` | Rickshaw integration: client/server scripts, parameter transformations |
| `multiplex.json` | Parameter validation rules, unit conversions, and presets for multiplex |
| `benchmark-metadata.json` | Machine-readable description and CDM-indexed source/type list (consumed by `crucible benchmarks list`) |
| `oslat-base` | Base setup shared by other scripts |
| `oslat-client` | Client-side benchmark execution |
| `oslat-server-start` / `oslat-server-stop` | Optional server lifecycle management |
| `oslat-get-runtime` | Extracts runtime from command-line options |
| `oslat-post-process.py` | Parses oslat output into crucible metrics |
| `client-workshop.json` / `server-workshop.json` | Engine image build requirements |

## Conventions
- Primary branch is `master`
- Standard Bash modelines and 4-space indentation
- Python code follows 4-space indentation with standard modelines
