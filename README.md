grunt-git-rev-parse
===================

A git tool for grunt 

> Get git commit id

## Getting Started
This plugin requires Grunt `~0.4.0`

First of all, you need to install this plugin by npm,
```shell
npm install grunt-git-rev-parse --save-dev
```
And second, you need to load this task in your grunt file.
```js
grunt.loadNpmTasks('grunt-git-rev-parse');
```

## The "git-describe" task

### Overview
In your project's Gruntfile, add a section named `git-rev-parse` to the data object passed into `grunt.initConfig()`.

```js
grunt.initConfig({
  "git-rev-parse": {
    "options": {
      // Task-specific options go here.
    }
  },
})
```

### Options

#### options.prop
Type: `String`  
Default value: `''`

A string value that is used as a property name for storing the result of this task

#### options.number
Type: `Number`  
Default value: `6`

The number of SHA1 value. Under the hood, this is the 'number' of git command `--short=[number]`

Inspired by Mikael Karon [grunt-git-describe](https://github.com/mikaelkaron/grunt-git-describe)
