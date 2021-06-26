# HeyRobot Thesaurus

This git repository includes:

- A tiny and simple JavaScript interface for querying Moby Thesaurus and Open Office Thesaurus data.
- A command-line interface (CLI) for searching a local, cached copy of the thesaurus from the terminal.

## Command Line Usage

Install [node.js](http://nodejs.org/) if you don't already have it. Then:

```sh
npm install moby --global
moby ecstasy
```

Display results one per line:

```sh
moby weird | tr , '\n'
```

## Node.js Usage

Install moby in your project directory. The `--save` flags adds it to the list of
`dependencies` in your package.json file.

```sh
cd my-project
npm install moby --save
```

Then in your javascript code:

```js
var moby = require('moby')

console.log(moby.search('mad'))
console.log(moby.search('smaragdine'))
console.log(moby.reverseSearch('smaragdine'))
```
