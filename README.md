hft-local
=========

Helps run an HTML based [HappyFunTimes game](http://greggman.github.io/HappyFunTimes) without HappyFunTimes

Why?
----

HappyFunTimes is a system that supports many players using there smartphones as controllers.
It's also a kind of virtual console and provides some common features like launching games,
quiting games, and other things. In order to allow HappyFunTimes to update its common
features it uses templates that insert the individual games content into an HTML frame at
runtime. This has the consequence that you can't run the games outside of HappyFunTimes.

Normally that's fine, most HappyFunTimes games require controllers and are basically not
meant to be played outside it's system but once in a while you'd like to be able to point
people to a live "demo"

For example

[http://greggman.github.io/hft-boomboom/...](http://greggman.github.io/hft-boomboom/local.html?settings=%7BhaveServer:false,numLocalPlayers:400,ai:true,waitForPlayersDuration:2,waitForStartDuration:2,bombStartSize:10,showFPS:true,showGithub:true%7D)

How To Use
----------

Install [bower](http://bower.io) then

    cd your-hft-project
    bower install hft-local

Then copy `bower_components/hft-local/local.html` to your local folder

    cp bower_components/hft-local/local.html .

Now run a local server and go to local.html.

Note: It's up to you to make your game run without networked players. See LocalNetPlayer
and/or look at the examples. Most of them use URL query parameters to decide whether to
manually spawn local players.

*   [BoomBoom](http://greggman.github.io/hft-boomboom/local.html?settings=%7BhaveServer:false,numLocalPlayers:400,ai:true,waitForPlayersDuration:2,waitForStartDuration:2,bombStartSize:10,showFPS:true,showGithub:true%7D)
*   [JumpJump](http://greggman.github.io/hft-jumpjump/local.html?settings=%7BhaveServer:false,numLocalPlayers:400,ai:true,waitForPlayersDuration:2,waitForStartDuration:2,bombStartSize:10,showFPS:true,showGithub:true%7D)
*   [PowPow](http://greggman.github.io/hft-powpow/local.html?settings=%7BhaveServer:false,numLocalPlayers:400,ai:true,waitForPlayersDuration:2,waitForStartDuration:2,bombStartSize:10,showFPS:true,showGithub:true%7D)

