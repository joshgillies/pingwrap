## Node.js Ping utility

A easy to use utility for node.js to send ping requests

##Installation

Install via npm

    $ npm install pingwrap

##Development

Make sure you have the latest node, coffee-script and npm installed.

The pingwrap source is located in src/ping.coffee

## Usage

First require it in your application

    var ping = require('pingwrap');

You can then call the ping function by passing it two arguments:

    ping( [hostname/ip], [callback] );


## Example:

    sys = require('util');
    ping = require('pingwrap');

    ping('google.com', function(error, stdout, stderr) {
      return sys.puts(stdout);
    });
