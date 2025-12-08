<h1 align="center">Azure Lab </h1>

<div align="center">
  This repository hosts my Azure labs. It’s intention is to be a space for learning and experimenting.
</div>


This repo contains my Azure labs, where I build and test different cloud setups. It is intended to be a playground for learning, experimenting, and making mistakes.

---

## Prerequisites
1. Debian WSL installed
2. Azure CLI installed and logged in:
```
curl -sL https://aka.ms/InstallAzureCLIDeb | sudo bash
```
```bash
az login --use-device-code
```
3. List available subscriptions:
```bash
az account list --output table
```
4. Set the subscription to use:
```bash
az account set --subscription <your-subscription-id>
```
5. Create SSH keys (on your local Linux environment):
```bash
ssh-keygen -t rsa -b 2048 -f ~/.ssh/azure_key
```
6. Terraform should be installed for deployments. Confirm with:
```bash
terraform -version
```

---

### Optional Notes

- All commands are designed to run locally on Linux (WSL or native).
- SSH keys are stored in `~/.ssh`
