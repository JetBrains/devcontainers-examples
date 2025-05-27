[![team project](http://jb.gg/badges/team.svg)](https://github.com/JetBrains#jetbrains-on-github)
[![License: Apache 2.0](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://www.apache.org/licenses/LICENSE-2.0)

# DevContainers Examples

A comprehensive collection of examples demonstrating how to use DevContainers with JetBrains IDEs.

## Table of Contents

- [Overview](#overview)
- [What are DevContainers?](#what-are-devcontainers)
- [Benefits of DevContainers](#benefits-of-devcontainers)
- [Repository Structure](#repository-structure)
- [Getting Started](#getting-started)
  - [Prerequisites](#prerequisites)
  - [Installation](#installation)
  - [Usage](#usage)
- [Examples](#examples)
  - [Minimal OS Examples](#minimal-os-examples)
  - [Specification Examples](#specification-examples)
  - [Demo Applications](#demo-applications)
  - [Customizations](#customizations)
  - [GPU Support](#gpu-support)
- [Troubleshooting](#troubleshooting)
- [Contributing](#contributing)
- [License](#license)

## Overview

This repository provides a collection of examples and templates for using DevContainers with JetBrains IDEs. It demonstrates various configurations, features, and use cases to help developers quickly set up reproducible development environments.

## What are DevContainers?

DevContainers (Development Containers) are a technology that allows developers to package a fully functional development environment inside containers. This approach ensures that all team members work with identical development environments, regardless of their local setup.

The DevContainers approach enables:

- Running applications in isolated environments
- Using IDEs and development tools consistently across the team
- Managing appropriate versions of libraries and dependencies
- Configuring runtimes required by specific codebases and projects
- Simplifying onboarding for new team members
- Utilizing remote development capabilities on servers with Docker and necessary hardware

## Benefits of DevContainers

- **Consistency**: Everyone on the team works with the same environment, eliminating "it works on my machine" problems
- **Efficiency**: Significantly reduces time spent setting up development environments
- **Onboarding**: New team members can start contributing quickly without extensive environment setup
- **Isolation**: Projects with different dependencies can coexist without conflicts
- **Portability**: Development environments can be easily moved between machines
- **Reproducibility**: Environments can be recreated exactly as needed for debugging or testing

JetBrains IDEs provide built-in support for DevContainers, allowing you to:
- Use pre-configured environments with required dependencies
- Create and customize your own DevContainers
- Access source code without manual uploading (via source mounting or creating a DevContainer from a repository over SSH)
- Enjoy the same developer experience as when working locally, thanks to Remote Development technology

## Repository Structure

This repository is organized into several main directories:

- **`minimalOS/`**: Contains minimal DevContainer configurations for various operating systems
- **`specification/`**: Demonstrates different DevContainer specification options and features
- **`demoApps/`**: Contains sample applications configured to run in DevContainers
- **`customizations/`**: Shows how to customize DevContainers with plugins and extensions
- **`gpu_amd64/`**: Provides examples for GPU support in DevContainers

## Getting Started

### Prerequisites

- Docker installed on your local machine
- A JetBrains IDE with DevContainers support (IntelliJ IDEA, PyCharm, WebStorm, etc.)
- [JetBrains DevContainers Plugin](https://plugins.jetbrains.com/plugin/21962-dev-containers)

### Installation

1. Clone this repository:
   ```bash
   git clone https://github.com/JetBrains/devcontainers-examples.git
   cd devcontainers-examples
   ```

2. Install the DevContainers plugin in your JetBrains IDE:
   - Go to Settings/Preferences > Plugins
   - Search for "Dev Containers"
   - Install the plugin and restart your IDE

### Usage

The DevContainer configuration is defined in a `devcontainer.json` file, which can be located in one of the following paths:

- `.devcontainer/devcontainer.json`
- `.devcontainer.json`
- `.devcontainer/<folder>/devcontainer.json` (where `<folder>` is a sub-folder, one level deep)

To build and run a DevContainer:

1. Open your project in a JetBrains IDE
2. The IDE will detect the DevContainer configuration and prompt you to reopen the project in a container
3. Click "Reopen in Container" to start the container build process
4. Once the container is built, your IDE will connect to it and you can start working

For detailed instructions, refer to the [official JetBrains documentation](https://www.jetbrains.com/help/idea/connect-to-devcontainer.html#start_from_gateway).

## Examples

### Minimal OS Examples

The `minimalOS/` directory contains examples for various Linux distributions:

- Alpine
- Ubuntu
- Debian
- Fedora
- AlmaLinux
- ArchLinux (AMD64 and ARM64)
- ClearLinux
- Gentoo
- Kali Linux
- Manjaro
- openSUSE
- Oracle Linux
- Rocky Linux

These examples provide a minimal setup for each operating system with the necessary dependencies for DevContainers.

### Specification Examples

The `specification/` directory contains examples demonstrating various DevContainer specification options:

- Port forwarding and attributes
- Environment variables
- User configuration
- Command overrides
- Security options
- Mounts and volumes
- Features and customizations
- Workspace configuration
- Lifecycle hooks
- Docker Compose integration

### Demo Applications

The `demoApps/` directory contains sample applications configured to run in DevContainers:

- `python-webserver/`: A Python web server example
- `static/`: A static website example

### Customizations

The `customizations/` directory demonstrates how to customize DevContainers:

- `plugins/`: Examples of configuring IDE plugins in DevContainers

### GPU Support

The `gpu_amd64/` directory provides examples for using GPUs in DevContainers.

## Troubleshooting

If you encounter any issues, please click "Help" → "Submit a bug report…" in the IDE and describe the problem—we’ll do our best to help.

## Contributing

Contributions to this repository are welcome! If you have an example or improvement to share, please submit a pull request.

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE.txt](LICENSE.txt) file for details.

Copyright 2025 JetBrains s.r.o. and respective authors and developers.
