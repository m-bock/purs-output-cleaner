# purs-output-cleaner

Have you ever got annoyed by receiving auto completions from already deleted modules in PureScript?
The reason is that those modules still hang around inside the output folder.

If you don't want to remove the output folder and do a full rebuild, you can use this tool. It cleans the output folder from non-existing modules.

## Installation

E.g:

```text
yarn global add https://github.com/thought2/purs-output-cleaner
```

## Usage

### As CLI

Inside a spago project folder:

```text
purs-output-cleaner
```

### In the IDE

Configure "Build Command" in the settings of the PureScript language extension:

`spago build --before purs-output-cleaner --purs-args --json-errors`

(Tested in vscode only)