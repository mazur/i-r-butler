I R Butler - IronRuby on Mono Installer
=======================================

This script is a result of the research I've made on how to build a complete working IronRuby installation from source on mono. 

I hope to make this a pain free way to get a fresh IronRuby install on any *nix system.

Right now it's pretty rough and you should probably not use it but I wanted to share my progress with everyone and hopefully save someone a couple of hours

Prerequisites
=============
* Mono 2.10 (or older compiled with C#4.0 support)
* Mono developer tools (dmcs & xbuild)
* GIT

What does it do so far?
=======================
So far the script will:

* Clone IronRuby from github.
* Build IronRuby
* Copy necessary files into the correct release structure
* Generate scripts for IronRuby

All files are placed into ~/.ironruby. To 'undo' the install you can just delete that folder.

Usage
=====
```bash
git clone git://github.com/mazur/i-r-butler.git
cd i-r-butler
./install
```

License
=======
Copyright (C) 2011 by Martin Mazur

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
