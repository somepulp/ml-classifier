# ml-classifier

Source code for the ML text classification service. Contains the Python application, model training pipeline, Dockerfile, and CI/CD workflow. On merge to main, CI builds and pushes a versioned image to Harbor and updates the image reference in platform-deploy to trigger a GitOps deployment.

Does not manage: Helm chart definitions (see `platform-charts`), deployment manifests or environment config (see `platform-deploy`), or infrastructure (see `platform-infra`).