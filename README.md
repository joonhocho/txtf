tstf
====

CLI tools for useful TypeScript code transformations such as paths transforms

[![oclif](https://img.shields.io/badge/cli-oclif-brightgreen.svg)](https://oclif.io)
[![Version](https://img.shields.io/npm/v/tstf.svg)](https://npmjs.org/package/tstf)
[![Downloads/week](https://img.shields.io/npm/dw/tstf.svg)](https://npmjs.org/package/tstf)
[![License](https://img.shields.io/npm/l/tstf.svg)](https://github.com/joonhocho/tstf/blob/master/package.json)

<!-- toc -->
* [Usage](#usage)
* [Commands](#commands)
<!-- tocstop -->
# Usage
<!-- usage -->
```sh-session
$ npm install -g tstf
$ tstf COMMAND
running command...
$ tstf (-v|--version|version)
tstf/0.0.1 darwin-x64 node-v11.10.0
$ tstf --help [COMMAND]
USAGE
  $ tstf COMMAND
...
```
<!-- usagestop -->
# Commands
<!-- commands -->
* [`tstf help [COMMAND]`](#tstf-help-command)
* [`tstf relToAlias`](#tstf-reltoalias)

## `tstf help [COMMAND]`

display help for tstf

```
USAGE
  $ tstf help [COMMAND]

ARGUMENTS
  COMMAND  command to show help for

OPTIONS
  --all  see all commands in CLI
```

_See code: [@oclif/plugin-help](https://github.com/oclif/plugin-help/blob/v2.2.0/src/commands/help.ts)_

## `tstf relToAlias`

transform relative paths to alias paths according to tsconfig.compilerOptions.paths

```
USAGE
  $ tstf relToAlias

OPTIONS
  -h, --help                                  show CLI help
  -p, --project=project                       (required) [default: tsconfig.json] path to tsconfig.json
  -q, --quote=s|d                             [default: d] whether to use single or double quote. default is d(ouble)
  -v, --verbose=0|1|2|3|debug|log|warn|error  verbose = debug | log (default) | warn | error
  -w, --write                                 whether to write to source files

EXAMPLES
  $ tstf relToAlias -p tsconfig.json
  $ tstf relToAlias -p tsconfig.json -q s -w -v
```

_See code: [src/commands/relToAlias.ts](https://github.com/joonhocho/tstf/blob/v0.0.1/src/commands/relToAlias.ts)_
<!-- commandsstop -->
