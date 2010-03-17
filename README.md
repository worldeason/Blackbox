Blackbox
========
Blackbox is an embeddable Cocoa HTTP server -- sort of: strictly speaking, it's a set of classes that wraps the terrific [CocoaHTTPServer][cocoahttp] project, which deserves all of the credit for the code that does the heavy-lifting. Blackbox allows you to associate HTTP resources with Cocoa "responder" objects (kind of like [Twisted Web](http://twistedmatrix.com/trac/wiki/TwistedWeb) does for Python) rather than files on your filesystem.

With Blackbox, you can create personal file sharers in a snap, write applications that communicate with each other over HTTP, and easily create web control interfaces for headless applications.

Want a demo? Check out [this (old) video](http://vimeo.com/3416746), which shows how you can build a small personal web server in under 15 minutes with Blackbox. (**Note**: don't rely on the API demonstrated in the video; the project works more or less the same way, but the method names have changed considerably since the video was created).

Documentation
-------------
Documentation is forthcoming, but not yet available. :) If you want to play around with it, start with the Blackbox Demo app, included in the project. **Please note** that the demo application links against the `SystemConfiguration` framework; this is *not necessary* to use Blackbox, the framework is only used to get the computer name to display as the placeholder text for "Bonjour Name." This value is obtained automatically if you set the Bonjour name to `nil`.

Projects That Use Blackbox
--------------------------
Currently the only known project that uses Blackbox is [Bowtie](http://bowtieapp.com) -- my themeable iTunes controller -- which uses Blackbox to communicate with Bowtie for iPhone and other remote clients.

Do you use Blackbox in your project? Drop me a note at m@13bold.com, and I'll add you to this list!

License
-------
Blackbox is licensed under the MIT license, excerpted below.

	Copyright (C) 2010 Matt Patenaude.

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

This project is a wrapper around the [CocoaHTTPServer project][cocoahttp], by Deusty Designs.

	Copyright (c) 2006, Deusty Designs, LLC
	All rights reserved.

	Redistribution and use of this software in source and binary forms,
	with or without modification, are permitted provided that the following conditions are met:

	* Redistributions of source code must retain the above
	  copyright notice, this list of conditions and the
	  following disclaimer.

	* Neither the name of Desuty Designs nor the names of its
	  contributors may be used to endorse or promote products
	  derived from this software without specific prior
	  written permission of Deusty Designs, LLC.

	THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT OWNER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.

  [cocoahttp]: http://code.google.com/p/cocoahttpserver/