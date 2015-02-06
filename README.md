# INIT Static Site Generator

A plugin for [INIT](http://use-init.com/) using [grunt-generator](https://www.npmjs.com/package/grunt-generator) to output a static site of your HTML partials.

[![devDependency Status](https://david-dm.org/init/init-static-site-generator/dev-status.png)](https://david-dm.org/use-init/init-static-site-generator#info=devDependencies)

## Installation
You can add this plugin to INIT by copying over the file `config/static-site-generator.js` to `tasks/options` and run

	npm install --save-dev grunt-generator

in your main project's root directory.

You need to add an object in your `config.js` file called `generator` to describe the files to be minimized:

	// Static Site Generator
	{
		files: {
			cwd: 'src/pages',
			src: '**/*',
			dest: 'dist/',
			ext: '.html'
		},
		options: {
			partialsglob: 'pages/partials/*.html',
			templates: 'src/templates',
			environment: 'dev'
		}
	}

**More info at and sample configuration: https://github.com/use-init/init/commit/c8dede58ba12ad283e388147d2f7ed869d40b9f2**

## Contribute
Please help making this project better and [contribute](CONTRIBUTING.md) with your knowledge.

## Development
This package is developed as part of the [INIT project](https://github.com/use-init).

## License
Please be aware of the licenses of each component we use in this project. Everything else that has been developed by the contributions to this project is under [MIT License](LICENSE.md).
