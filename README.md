# cipher-repo

The official APT package repository for **CIPHER Linux**, hosting optional metapackages not included in the base ISO.

**Live at:** https://cipher-linux.github.io/cipher-repo

## Add this repo

```bash
echo "deb [trusted=yes] https://cipher-linux.github.io/cipher-repo stable main" | sudo tee /etc/apt/sources.list.d/cipher-repo.list
sudo apt update
```

## Available metapackages

| Package | Purpose |
|---|---|
| `cipher-admin` | System administration tools |
| `cipher-network` | Networking utilities |
| `cipher-security` | Security & pentesting tools |
| `cipher-forensics` | Digital forensics tools |
| `cipher-dev` | Development tools |
| `cipher-devops` | DevOps tools |

Install any of these like a normal package, e.g.:

```bash
sudo apt install cipher-security
```

## How this repo is maintained

Packages are built and signed, then published here via `reprepro`. GPG signature verification is enabled — apt will validate packages against the CIPHER Linux signing key automatically.

---
Part of the [CIPHER Linux](https://github.com/cipher-linux) project.
