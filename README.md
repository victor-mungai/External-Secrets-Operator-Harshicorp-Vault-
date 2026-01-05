# HashiCorp Vault + External Secrets Operator (Kubernetes)

This repository demonstrates how to integrate HashiCorp Vault with Kubernetes using the External Secrets Operator (ESO) to sync secrets from Vault into native Kubernetes Secrets.

The setup uses:

Vault (running via Docker)

External Secrets Operator

A ClusterSecretStore connected to Vault

An ExternalSecret that materializes a Vault secret inside Kubernetes

The goal is to show a minimal, working setup that’s easy to understand and reproduce.

#📁 Repository Structure
```
├── docker-compose.yaml        # Runs Vault locally
├── cluster-secretstore.yaml   # Vault backend configuration for ESO
├── external-secret.yaml       # Pulls a secret from Vault into Kubernetes
```
# Full Walkthrough

For the complete, step-by-step guide — including:

Vault setup

Secret engine configuration

Authentication tradeoffs

How ESO actually creates Kubernetes Secrets

Debugging tips (and a bit of banter 😄)

 Read the full blog post on Medium: https://medium.com/@mungaivictor2781/i-finally-wired-hashicorp-vault-to-kubernetes-using-external-secrets-operator-and-lived-to-tell-af90b133cabb

# Notes

This project is intended for learning and demos.

Some choices (like authentication method) are deliberately simplified to keep the focus on understanding how the integration works.
