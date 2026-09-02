<!-- repo-header:start -->
<img src="https://github.com/writerslogic.png?size=160" alt="Add the bucket logo" width="120" align="left">

<h1>Add the bucket</h1>

<p><strong>Scoop bucket for CPoE (Windows)</strong></p>

<br clear="left">

[![CI](https://img.shields.io/github/actions/workflow/status/writerslogic/scoop-bucket/excavator.yml?style=flat-square&labelColor=20232a&branch=main&label=CI)](https://github.com/writerslogic/scoop-bucket/actions/workflows/excavator.yml) [![Best Practices Evidence](https://img.shields.io/badge/best%20practices-evidence%20reviewed-6a4c93?style=flat-square&labelColor=20232a)](.bestpractices.json) [![GitHub Sponsors](https://img.shields.io/badge/GitHub%20Sponsors-Sponsor-EA4AAA?style=flat-square&labelColor=20232a)](https://github.com/sponsors/dcondrey)
<!-- repo-header:end -->

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
