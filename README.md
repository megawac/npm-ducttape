# npm-ducttape

A simple script to ducttape your dependencies into a subfolder of your package, so they can be installed without NPM registry on deploy.

**NB! Due to changes in NPM install in version 3.10.8 then shrinkwrap generated with 3.10.8 will not work with earlier versions and vice versa.**

## Installation

Prefer installing globally as installing locally will require you to also add it to package.json as a dependency - otherwise shrinkwrap **WILL** fail.

    npm install -g npm-ducttape

## Usage

### Global

    npm-ducttape
    
Or if you want to specify a folder

    npm-ducttape my-fancy-folder
    
## Options

### --dev

You can provide the *--dev* flag to *npm-ducttape*. This flag will be passed on to shrinkwrap to include devDependencies in the build.

    npm-ducttape --dev

You can provide both a custom folder and the --dev flag

    npm-ducttape my-fancy-folder --dev
    

## TODO:

1. More tests

## License

The MIT License (MIT)
Copyright (c) 2016 Karl Düüna

Permission is hereby granted, free of charge, to any person obtaining a copy of
this software and associated documentation files (the "Software"), to deal in
the Software without restriction, including without limitation the rights to
use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of
the Software, and to permit persons to whom the Software is furnished to do so,
subject to the following conditions:

The above copyright notice and this permission notice shall be included in all
copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
SOFTWARE.