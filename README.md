oclif-hello-world
=================

oclif example Hello World CLI

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![CircleCI](https://circleci.com/gh/oclif/hello-world/tree/main.svg?style=shield)](https://circleci.com/gh/oclif/hello-world/tree/main)
[![Downloads/week](https://img.shields.io/npm/dw/oclif-hello-world.svg)](https://npmjs.org/package/oclif-hello-world)
[![License](https://img.shields.io/npm/l/oclif-hello-world.svg)](https://github.com/oclif/hello-world/blob/main/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g my-oclif-plugin
$ my-oclif-plugin COMMAND
running command...
$ my-oclif-plugin (--version)
my-oclif-plugin/0.0.0 darwin-arm64 node-v18.10.0
$ my-oclif-plugin --help [COMMAND]
USAGE
  $ my-oclif-plugin COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`my-oclif-plugin hello PERSON`](#my-oclif-plugin-hello-person)
* [`my-oclif-plugin hello world`](#my-oclif-plugin-hello-world)
* [`my-oclif-plugin help [COMMAND]`](#my-oclif-plugin-help-command)
* [`my-oclif-plugin plugins`](#my-oclif-plugin-plugins)
* [`my-oclif-plugin plugins:install PLUGIN...`](#my-oclif-plugin-pluginsinstall-plugin)
* [`my-oclif-plugin plugins:inspect PLUGIN...`](#my-oclif-plugin-pluginsinspect-plugin)
* [`my-oclif-plugin plugins:install PLUGIN...`](#my-oclif-plugin-pluginsinstall-plugin-1)
* [`my-oclif-plugin plugins:link PLUGIN`](#my-oclif-plugin-pluginslink-plugin)
* [`my-oclif-plugin plugins:uninstall PLUGIN...`](#my-oclif-plugin-pluginsuninstall-plugin)
* [`my-oclif-plugin plugins:uninstall PLUGIN...`](#my-oclif-plugin-pluginsuninstall-plugin-1)
* [`my-oclif-plugin plugins:uninstall PLUGIN...`](#my-oclif-plugin-pluginsuninstall-plugin-2)
* [`my-oclif-plugin plugins update`](#my-oclif-plugin-plugins-update)

## `my-oclif-plugin hello PERSON`

Say hello

```
USAGE
  $ my-oclif-plugin hello [PERSON] -f <value>

ARGUMENTS
  PERSON  Person to say hello to

FLAGS
  -f, --from=<value>  (required) Who is saying hello

DESCRIPTION
  Say hello

EXAMPLES
  $ oex hello friend --from oclif
  hello friend from oclif! (./src/commands/hello/index.ts)
```

_See code: [dist/commands/hello/index.ts](https://github.com/shunsukew/my-oclif-plugin/blob/v0.0.0/dist/commands/hello/index.ts)_

## `my-oclif-plugin hello world`

Say hello world

```
USAGE
  $ my-oclif-plugin hello world

DESCRIPTION
  Say hello world

EXAMPLES
  $ my-oclif-plugin hello world
  hello world! (./src/commands/hello/world.ts)
```

## `my-oclif-plugin help [COMMAND]`

Display help for my-oclif-plugin.

```
USAGE
  $ my-oclif-plugin help [COMMAND] [-n]

ARGUMENTS
  COMMAND  Command to show help for.

FLAGS
  -n, --nested-commands  Include all nested commands in the output.

DESCRIPTION
  Display help for my-oclif-plugin.
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v5.1.15/src/commands/help.ts)_

## `my-oclif-plugin plugins`

List installed plugins.

```
USAGE
  $ my-oclif-plugin plugins [--core]

FLAGS
  --core  Show core plugins.

DESCRIPTION
  List installed plugins.

EXAMPLES
  $ my-oclif-plugin plugins
```

_See code: [@oclif/plugin-plugins](https://github.com/oclif/plugin-plugins/blob/v2.1.2/src/commands/plugins/index.ts)_

## `my-oclif-plugin plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ my-oclif-plugin plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ my-oclif-plugin plugins add

EXAMPLES
  $ my-oclif-plugin plugins:install myplugin 

  $ my-oclif-plugin plugins:install https://github.com/someuser/someplugin

  $ my-oclif-plugin plugins:install someuser/someplugin
```

## `my-oclif-plugin plugins:inspect PLUGIN...`

Displays installation properties of a plugin.

```
USAGE
  $ my-oclif-plugin plugins:inspect PLUGIN...

ARGUMENTS
  PLUGIN  [default: .] Plugin to inspect.

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Displays installation properties of a plugin.

EXAMPLES
  $ my-oclif-plugin plugins:inspect myplugin
```

## `my-oclif-plugin plugins:install PLUGIN...`

Installs a plugin into the CLI.

```
USAGE
  $ my-oclif-plugin plugins:install PLUGIN...

ARGUMENTS
  PLUGIN  Plugin to install.

FLAGS
  -f, --force    Run yarn install with force flag.
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Installs a plugin into the CLI.
  Can be installed from npm or a git url.

  Installation of a user-installed plugin will override a core plugin.

  e.g. If you have a core plugin that has a 'hello' command, installing a user-installed plugin with a 'hello' command
  will override the core plugin implementation. This is useful if a user needs to update core plugin functionality in
  the CLI without the need to patch and update the whole CLI.


ALIASES
  $ my-oclif-plugin plugins add

EXAMPLES
  $ my-oclif-plugin plugins:install myplugin 

  $ my-oclif-plugin plugins:install https://github.com/someuser/someplugin

  $ my-oclif-plugin plugins:install someuser/someplugin
```

## `my-oclif-plugin plugins:link PLUGIN`

Links a plugin into the CLI for development.

```
USAGE
  $ my-oclif-plugin plugins:link PLUGIN

ARGUMENTS
  PATH  [default: .] path to plugin

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Links a plugin into the CLI for development.
  Installation of a linked plugin will override a user-installed or core plugin.

  e.g. If you have a user-installed or core plugin that has a 'hello' command, installing a linked plugin with a 'hello'
  command will override the user-installed or core plugin implementation. This is useful for development work.


EXAMPLES
  $ my-oclif-plugin plugins:link myplugin
```

## `my-oclif-plugin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ my-oclif-plugin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-oclif-plugin plugins unlink
  $ my-oclif-plugin plugins remove
```

## `my-oclif-plugin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ my-oclif-plugin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-oclif-plugin plugins unlink
  $ my-oclif-plugin plugins remove
```

## `my-oclif-plugin plugins:uninstall PLUGIN...`

Removes a plugin from the CLI.

```
USAGE
  $ my-oclif-plugin plugins:uninstall PLUGIN...

ARGUMENTS
  PLUGIN  plugin to uninstall

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Removes a plugin from the CLI.

ALIASES
  $ my-oclif-plugin plugins unlink
  $ my-oclif-plugin plugins remove
```

## `my-oclif-plugin plugins update`

Update installed plugins.

```
USAGE
  $ my-oclif-plugin plugins update [-h] [-v]

FLAGS
  -h, --help     Show CLI help.
  -v, --verbose

DESCRIPTION
  Update installed plugins.
```
<!-- commandsstop -->
# my-oclif-plugin
