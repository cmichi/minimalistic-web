# Minimalistic Web

Many websites are overloaded with features. This effectively makes them less 
usable. This project aims on providing templates for stripping websites down 
to the most necessary stuff.
I have written a description of the concept down 
[here](http://micha.elmueller.net/2013/04/the-aesthetics-of-simplicity/).

Before/After screenshots are posted on this tumblr: 
[minimalistic-web.tumblr.com](http://minimalistic-web.tumblr.com).


__Note__: The templates 

 * are designed for the [Privoxy](http://www.privoxy.org/) web proxy
 * are not executed for websites you access over HTTPS
 * are designed to be used in conjunciton with an AdBlock Browser Addon


# Installation

Install and configure Privoxy. For Ubuntu e.g. `$ sudo apt-get install privoxy`.

Install AdBlock, either as an 
[AdBlock Browser Addon](http://adblockplus.org/de/firefox) or as templates
for Privoxy (I followed the instructions provided
[here](https://github.com/skroll/privoxy-adblock)).

Clone the repo `$ git clone https://github.com/cmichi/minimalistic-web.git`.

Append to `/etc/privoxy/config`:

	actionsfile /path-to-repo/minimalistic.action
	filterfile /path-to-repo/minimalistic.filter

Restart Privoxy `$ sudo /etc/init.d/privoxy restart` (Ubuntu) and make sure
your browser is configured to use the proxy. Et voilà!

In case of the templates not being loaded you might have to move them into
a subdirectory of /etc/privoxy/.


# Supported Sites so far

 * MediaWiki: you need to add the URI of the Wiki to `minimalistic.action`,
   german and english Wikipedia are there as a default.
 * spiegel.de
 * golem.de
 * ~~zeit.de~~ (zeit stylesheet was changed in the meantime, needs rework)


# ToDo 

 * create gallery/showcase of berfore/after templating of websites
 * Ideas for sites to "redesign": soup.io fullscreen view, wetter.de


# License

This project is licensed under MIT:

	Copyright (c) 2013-2014 

		Michael Mueller, <http://micha.elmueller.net/>
	
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
