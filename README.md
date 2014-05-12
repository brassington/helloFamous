#hellofamous                                                                                                               
> Seed project to get started with Famo.us created by Grunt.

##Dependencies
It is actually quite simple really

First make sure you have node.js, grunt-cli, and bower installed.

```
brew install node
npm install -g grunt-cli bower
```

If you are installing node for the fist time you will most likely need to add npm to your path

```
$ export PATH="/usr/local/share/npm/bin:$PATH"
```

You will probably want to add that to you .bash_profile.  I'll assume if you are using any other shell that you know what you are doing already :P

##Getting Started

```
npm install && bower install
```

That's it!!!

##Running the Development Server

Simply run ```grunt serve``` and you will start a local development server and open Chrome.  Watch tasks will be running, and your browser will be automatically refreshed whenever a file in the repo changes.

You can run serve with ```--port=9001``` to manually pick the port that the server will run on

##Production

If you would like to compile your project for distribution simply run the command ```grunt``` to build ```dist/``` which will be a deployment ready version of your app.  Preprocessing will be applied to html, all js will be concatenated and minified.  All js / css assets will also have their name prepended with a hash for cache busting.

##Why are styles so strict?

While the default style guidelines are fairly strict, we are doing so with reason.  Famo.us is not only a framework for creating cutting edge web application, but a community project that we are all going to contribute to in the hopes of making the web better.  We truly believe that having consistent style within the community will make it easier for individuals to jump between different Famo.us modules without having to waste valuable time on processing style.

While our Package Manager (which is currently in development) will enforce our style guide if you would like to publish a module, feel free to disable eslint or jscs as you see fit.  If you want to disable linting you will need to comment out lines 57 (lint during watch task), 250-251 (run when server is launched), and 260-261 (lint when building for production)

## Contributing
All contributions are welcome! The simplest way to show your support for this project is to **"star" it**.

## Release History
 * 2014-04-10   v0.1.0   Generated by the [Yeoman Generator](https://github.com/famous/generator-famous) for [Famo.us](http://famo.us)
