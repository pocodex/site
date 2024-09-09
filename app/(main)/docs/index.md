# Overview

pocodex is a PocketBase plugin architecture and ecosystem. It is a central location where developers can submit and maintain pocodex-compatible plugins that extend the core functionality of PocketBase. pocodex installs a `codex` command into the PocketBase CLI, making it easy to manage plugins.

## Installation

To install pocodex, use the following command:

```bash
bun add pocodex
```

## Usage

Once installed, you can use the `codex` command to manage plugins:

- **List all available plugins (global)**:

  ```bash
  pocketbase codex list --global
  # or
  pocketbase codex ls --global
  ```

- **List installed plugins**:

  ```bash
  pocketbase codex list
  # or
  pocketbase codex ls
  ```

- **Install a plugin**:

  ```bash
  pocketbase codex install <plugin>
  # or
  pocketbase codex i <plugin>
  ```

- **Uninstall a plugin**:

  ```bash
  pocketbase codex uninstall <plugin>
  # or
  pocketbase codex u <plugin>
  ```

- **Search for plugins by keyword**:

  ```bash
  pocketbase codex search <keyword>
  ```

- **Enable a disabled plugin**:

  ```bash
  pocketbase codex enable <plugin>
  ```

- **Disable a plugin without uninstalling**:
  ```bash
  pocketbase codex disable <plugin>
  ```

## Creating Plugins

See the [Plugin Authoring Guide](/authoring)
