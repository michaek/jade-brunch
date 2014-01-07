## jade-brunch
Adds [Jade](http://jade-lang.com) support to [brunch](http://brunch.io), by 
compiling templates into dynamic javascript modules.

## Usage
Install the plugin via npm with `npm install --save jade-brunch`.

Or, do manual install:

* Add `"jade-brunch": "x.y.z"` to `package.json` of your brunch app.
  Pick a plugin version that corresponds to your minor (y) brunch version.
* If you want to use git version of plugin, add
`"jade-brunch": "git+ssh://git@github.com:brunch/jade-brunch.git"`.

### Static HTML

You may also compile to static HTML by setting `static` on the plugin 
configuration:

    plugins:
      jade:
        static: true

In Brunch < 1.8.0, this will concatenate all matched HTML files,
which probably isn't what you want. Beginning in Brunch 1.8.0, the
filesets feature has a `separate` option, as described 
[here](https://github.com/brunch/brunch/issues/616).

## Assumptions

When using Jade's basedir relative `include` and `extend`, the basedir will be assumed to be 'app' within the Brunch root. See [#989](https://github.com/visionmedia/jade/pull/989)

## License

The MIT License (MIT)

Copyright (c) 2012-2013 Paul Miller (http://paulmillr.com)

Permission is hereby granted, free of charge, to any person obtaining a copy
of this software and associated documentation files (the "Software"), to deal
in the Software without restriction, including without limitation the rights
to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
copies of the Software, and to permit persons to whom the Software is
furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN
THE SOFTWARE.
