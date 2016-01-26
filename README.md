MS Edge iframe Web Audio bug
===========================

When an iframe that is playing audio using the Web Audio API is removed from the dom, it continues playing the audio.

In this particular example, it seems to stop after clicking on the page, but I have other another, more complex app where this is not the case, though I'm assuming it's the same issue.

To use, just run any simple HTTP server on this folder and visit in MS Edge. Clicking "No Audio" should stop the audio immediately, but it doesn't.

A workaround is to set the src of the iframe to an empty string before removing it.
