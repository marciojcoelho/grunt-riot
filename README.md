# grunt-riot

> grunt plugin for riot

This plugin compile [riot](https://github.com/muut/riotjs)'s `.tag` files.

## Getting Started
This plugin requires Grunt.

```shell
npm install grunt-riot --save-dev
```

Once that's done, add this line to your project's Gruntfile :

```js
grunt.loadNpmTasks('grunt-riot');
```
Or use [load-grunt-tasks](https://github.com/sindresorhus/load-grunt-tasks)


### Usage Examples

```js
grunt.initConfig({
  riot: {
    expand: true,
    cwd: '<%= app %>/scripts',
    src: '**/*.tag',
    dest: '<%= app %>/scripts',
    ext: '.js'
  },
})
```

### Options
* compact: `Boolean`
	* no whitespace between tags
	* default : `True`
* expr: `Boolean`
	* expressions trough parser
	* default : `True`
* type: `String`
	* javaScript parser type
	* default : `null`
* template: `String`
	* template parser
	* default : `null`
* parser: `Function`
	* custom javascript parser method
	* default : `null`


## Release History
2015-01-26  0.0.1

## License
Copyright (c) 2015 . Licensed under the MIT license.
