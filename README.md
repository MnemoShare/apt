# MnemoShare APT Repository

Official APT repository for MnemoShare packages.

## Installation

### Ubuntu/Debian

```bash
# Add MnemoShare repository
curl -fsSL https://mnemoshare.github.io/apt/pubkey.gpg | sudo gpg --dearmor -o /usr/share/keyrings/mnemoshare-archive-keyring.gpg

echo "deb [signed-by=/usr/share/keyrings/mnemoshare-archive-keyring.gpg] https://mnemoshare.github.io/apt stable main" | sudo tee /etc/apt/sources.list.d/mnemoshare.list

# Update and install
sudo apt update
sudo apt install mnemocli -y
```

### Verify Installation

```bash
mnemocli --version
```

## Available Packages

- **mnemocli** - MnemoShare CLI for HIPAA-compliant secure file transfers

## Support

- Homepage: https://github.com/mnemoshare/mnemoshare
- Issues: https://github.com/mnemoshare/mnemoshare/issues
