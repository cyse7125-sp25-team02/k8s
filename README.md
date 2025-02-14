# Kubernetes Manifests

## Prerequisites

- age
- sops
- kubectl

## Setup

1. Install required tools
2. Copy age public key from administrator
3. Create .sops.yaml with provided public key
4. Never commit unencrypted secrets

## Usage

- To decrypt secrets:
  sops --decrypt /base/secrets.enc.yaml

- To encrypt new secrets:
  sops --encrypt new-secrets.yaml > new-secrets.enc.yaml
