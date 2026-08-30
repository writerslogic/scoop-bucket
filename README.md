<p align="center">
  <strong>Scoop Bucket for WritersProof</strong><br>
  <em>Cryptographic authorship witnessing for writers and creators</em>
</p>

<p align="center">
  <a href="https://github.com/writerslogic/scoop-bucket/actions/workflows/ci.yml"><img src="https://github.com/writerslogic/scoop-bucket/actions/workflows/ci.yml/badge.svg" alt="Tests"></a>
  <a href="https://github.com/writerslogic/scoop-bucket/actions/workflows/excavator.yml"><img src="https://github.com/writerslogic/scoop-bucket/actions/workflows/excavator.yml/badge.svg" alt="Excavator"></a>
</p>

---

## What is WritersProof?

**WritersProof** creates tamper-evident cryptographic records of document authorship. It provides irrefutable proof that you wrote what you wrote, when you wrote it.

- **Prove authorship** — Cryptographic evidence chain linking you to your work
- **Detect AI content** — Forensic analysis identifies non-human writing patterns
- **Hardware-backed** — TPM 2.0 integration for device binding
- **Verify independently** — Evidence can be verified by anyone, anywhere

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
