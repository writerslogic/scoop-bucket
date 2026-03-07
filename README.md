<p align="center">
  <img src="https://raw.githubusercontent.com/writerslogic/witnessd/main/assets/logo.svg" alt="WritersLogic" width="300">
</p>

<p align="center">
  <strong>Scoop Bucket for WritersLogic</strong><br>
  <em>Cryptographic authorship witnessing for writers and creators</em>
</p>

<p align="center">
  <a href="https://github.com/writerslogic/scoop-bucket/actions/workflows/ci.yml"><img src="https://github.com/writerslogic/scoop-bucket/actions/workflows/ci.yml/badge.svg" alt="Tests"></a>
  <a href="https://github.com/writerslogic/scoop-bucket/actions/workflows/excavator.yml"><img src="https://github.com/writerslogic/scoop-bucket/actions/workflows/excavator.yml/badge.svg" alt="Excavator"></a>
  <a href="https://github.com/writerslogic/witnessd/releases/latest"><img src="https://img.shields.io/github/v/release/writerslogic/witnessd?label=version" alt="Version"></a>
  <a href="https://github.com/writerslogic/witnessd/blob/main/LICENSE"><img src="https://img.shields.io/badge/license-AGPL--3.0-blue" alt="License"></a>
</p>

---

## What is WritersLogic?

**WritersLogic** creates tamper-evident cryptographic records of document authorship. It provides irrefutable proof that you wrote what you wrote, when you wrote it.

- **Prove authorship** — Cryptographic evidence chain linking you to your work
- **Detect AI content** — Forensic analysis identifies non-human writing patterns
- **Hardware-backed** — TPM 2.0 integration for device binding
- **Verify independently** — Evidence can be verified by anyone, anywhere

## Installation

```powershell
# Add the bucket
scoop bucket add writerslogic https://github.com/writerslogic/scoop-bucket

# Install WritersLogic
scoop install writerslogic
```

## Quick Start

```powershell
# Initialize WritersLogic
wld init

# Calibrate VDF for your machine
wld calibrate

# Create checkpoints as you write
wld commit document.md -m "First draft"

# View history
wld log document.md

# Export evidence
wld export document.md --tier enhanced

# Verify evidence
wld verify evidence-packet.json

# Or verify online without installing:
# https://writerslogic.com/verify
```

## Updating

```powershell
# Update WritersLogic to the latest version
scoop update writerslogic
```

## Available Commands

After installation, both commands are available:

| Command | Description |
|---------|-------------|
| `wld` | Short alias (recommended) |
| `writerslogic` | Full binary name |

## Auto-Updates

This bucket includes an automated workflow that checks for new WritersLogic releases every 6 hours and updates the manifest automatically.

## Verification

All WritersLogic releases include:
- SHA256 checksums
- SLSA Level 3 provenance attestations
- SBOM (SPDX and CycloneDX)

## Other Platforms

| Platform | Installation |
|----------|--------------|
| macOS | `brew install writerslogic/tap/writerslogic` |
| From Source | See [build instructions](https://github.com/writerslogic/witnessd#from-source) |

## Links

- [WritersLogic Repository](https://github.com/writerslogic/witnessd)
- [Documentation](https://github.com/writerslogic/witnessd#readme)
- [Report Issues](https://github.com/writerslogic/witnessd/issues)
- [Website](https://writerslogic.com)

## License

WritersLogic is licensed under the [GNU Affero General Public License v3.0](https://github.com/writerslogic/witnessd/blob/main/LICENSE).
