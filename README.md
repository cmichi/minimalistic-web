# Minimalistic Web

Many websites are overloaded with features. This effectively makes them less 
usable. This project aims on providing templates for stripping websites down 
to the most necessary stuff.

The templates are for the [Privoxy](http://www.privoxy.org/) web proxy.

__Note__: Templates are not executed for websites you access over HTTPS!


# ToDo 

 * create gallery/showcase of berfore/after templating of websites


# Installation

Install Privoxy. For Ubuntu e.g.:

	# install privoxy
	$ sudo apt-get install privoxy

Clone the repo

	$ git clone https://github.com/cmichi/minimalistic-web.git 

and append to `/etc/privoxy/config`:

	actionsfile /path-to-repo/minimalistic.action
	filterfile /path-to-repo/minimalistic.filter

And at last restart Privoxy:

	$ sudo /etc/init.d/privoxy restart


# Supported Sites

 * spiegel.de
 * golem.de
 * MediaWiki


# License

This project is licensed under MIT:

	Copyright (c) 2013 Michael Mueller, <http://micha.elmueller.net/>
	
	Permission is hereby granted, free of charge, to any person obtaining
	a copy of this software and associated documentation files (the
	"Software"), to deal in the Software without restriction, including
	without limitation the rights to use, copy, modify, merge, publish,
	distribute, sublicense, and/or sell copies of the Software, and to
	permit persons to whom the Software is furnished to do so, subject to
	the following conditions:

	The above copyright notice and this permission notice shall be
	included in all copies or substantial portions of the Software.

	THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND,
	EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF
	MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND
	NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE
	LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION
	OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION
	WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.
