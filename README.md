# Codespaces Ionic Template

![Ionic](https://img.shields.io/badge/Ionic-3880FF?style=flat-square&logo=ionic&logoColor=white)
![GitHub Codespaces](https://img.shields.io/badge/GitHub_Codespaces-000000?style=flat-square&logo=github&logoColor=white)
![Ubuntu](https://img.shields.io/badge/Ubuntu-E95420?style=flat-square&logo=ubuntu&logoColor=white)
![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg?style=flat-square)
![Last Commit](https://img.shields.io/github/last-commit/danielcregg/codespaces-ionic-template?style=flat-square)

A GitHub Codespaces dev container template that provides a pre-configured cloud development environment for Ionic framework projects. Open a Codespace from this template and start building Ionic apps immediately with zero local setup.

## Features

- Pre-configured Ubuntu-based dev container
- Ionic CLI installed and ready to use
- npm automatically updated to the latest version on container creation
- Works entirely in the browser via GitHub Codespaces

## Prerequisites

- A GitHub account with access to [GitHub Codespaces](https://github.com/features/codespaces)

## Getting Started

1. Click the green **"Code"** button on this repository
2. Select the **"Codespaces"** tab
3. Click **"Create codespace on main"**
4. Wait for the container to build (first launch takes a few minutes)

Once the Codespace is ready, you can create a new Ionic project:

```bash
ionic start my-app blank --type=angular
cd my-app
ionic serve
```

## Dev Container Configuration

The template uses the following configuration:

| Setting | Value |
|---------|-------|
| Base Image | `mcr.microsoft.com/devcontainers/base:latest` (Ubuntu) |
| Ionic CLI | Latest version via dev container feature |
| Post-Create | Runs `npm install -g npm@latest` to ensure up-to-date npm |

## Project Structure

```
codespaces-ionic-template/
└── .devcontainer/
    └── devcontainer.json   # Dev container configuration
```

## Customization

To modify the dev container, edit `.devcontainer/devcontainer.json`. You can add additional VS Code extensions, features, or post-create commands as needed.

## License

This project is licensed under the MIT License. See the [LICENSE](LICENSE) file for details.
