# Arix Theme — Blueprint Framework Fork

## Introduction
**Arix Theme** is a customized fork of the Blueprint extension framework for Pterodactyl, tailored for seamless integration with the [Arix Theme](https://arix.gg). This fork adds automatic compatibility with Arix and maintains the powerful extension system Blueprint is known for.

### Install
Refer to the [installation guide](https://github.com/royaldevlopments/blueprint-framework).

<br>

## What's in here?
This repository hosts the framework patch that you apply onto your Pterodactyl panel. This overwrites files like installing a "standalone addon" would, but instead of being just that, the framework allows your panel to be extended through "extensions".

- The CLI is written in Bash.
- The backend adds onto Pterodactyl's, and is written in PHP/Laravel.
- The user-side frontend adds onto Pterodactyl's, and is written in React/TypeScript.
- The admin-side frontend adds onto Pterodactyl's, and is written in PHP/Laravel/Blade.

### CLI
Our main CLI script is [`blueprint.sh`](./blueprint.sh). This script gets called by `/usr/local/bin/blueprint` whenever a user runs the `blueprint` command, or queries bash autocomplete.

[`blueprint.sh`](./blueprint.sh) is in charge of the following duties;
- Finishing initial installation steps and updates (flushing cache, artisan commands, etc)
- Sourcing CLI dependencies ([`scripts/libraries`](./scripts/libraries))
- Running the right sub-scripts for each command ([`scripts/commands`](./scripts/commands))
- Placing the `blueprint` command shortcut to `/usr/local/bin/blueprint`

<br>
