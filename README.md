jquery.asyncQueue.js
====================

Usage
-----

// pre-initialize a global queue (before jquery.asyncQueue.js)
    window.queue = window.queue || [];

// queueing an anonymous function
    window.queue.push( function(){
        //code
    });

// queueing a standard function with scope and arguments
    window.queue.push( [
        console.log
        ,window
        ,firstArg
        ,secondArg
        //...
    ]);

// initializing queue (and executing its contents)
    $(window).aqueue('queue');
