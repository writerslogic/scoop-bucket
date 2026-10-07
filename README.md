### WritersProof Scoop Bucket

Scoop bucket for the CPoE CLI on Windows.

[![CI](https://img.shields.io/github/actions/workflow/status/writerslogic/scoop-bucket/ci.yml?branch=main&label=CI)](https://github.com/writerslogic/scoop-bucket/actions/workflows/ci.yml)

## Installation

```powershell
# Add the bucket
scoop bucket add writerslogic https://github.com/writerslogic/scoop-bucket

# Install the WritersProof CLI
scoop install writerslogic
```

> The package is named `writerslogic` after the bucket. The binary it installs is
> `writersproof-cli`.

## Quick Start

```powershell
# Initialize WritersProof
writersproof-cli init

# Calibrate VDF for your machine
writersproof-cli calibrate

# Create checkpoints as you write
writersproof-cli commit document.md -m "First draft"

# View history
writersproof-cli log document.md

# Export evidence
writersproof-cli export document.md --tier enhanced

# Verify evidence
writersproof-cli verify evidence-packet.json

# Or verify online without installing:
# https://writersproof.com/verify
```

## Updating

```powershell
scoop update writerslogic
```

## Other Platforms

| Platform | Installation |
|----------|--------------|
| macOS | `brew install writerslogic/tap/writersproof` |
| macOS / Linux | `curl -sSf https://writersproof.com/install.sh \| sh` |

## Links

- [Website](https://writersproof.com)
- [Downloads](https://writersproof.com/download)
- [Report Issues](https://github.com/writerslogic/writersproof-support/issues)

## License

The WritersProof CLI is licensed under the GNU Affero General Public License v3.0.
