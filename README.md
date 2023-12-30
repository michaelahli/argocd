# Argo CD Managed Applications Repository

This repository contains manifests for applications managed by Argo CD.

## Usage

1. **Install Argo CD:**
   Ensure that Argo CD is installed in your Kubernetes cluster. Follow the official Argo CD installation guide if not already installed.

2. **Add Repository:**
   Add this repository to your Argo CD instance:

   ```bash
   argocd repo add argo-apps-repo https://github.com/michaelahli/argocd
   ```

3. **Sync Applications:**
   Use Argo CD to sync applications from this repository. For example:

   ```bash
   argocd app sync my-application
   ```

   Replace `my-application` with the name of the application you want to sync.

## Structure

- Each application has its own directory containing Argo CD Application YAML files.
- Customize application configurations in the respective YAML files.
- Follow best practices for managing Kubernetes manifests within Argo CD.

## Contributing

Feel free to contribute by adding new applications, improving existing ones, or fixing issues. Create pull requests for changes.
