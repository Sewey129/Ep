// ==UserScript==
// @name         Hang Page
// @namespace    http://tampermonkey.net/
// @version      0.1
// @description  Hang the page for a specified amount of time.
// @author       You
// @match        https://www.educationperfect.com/
// @grant        none
// ==/UserScript==

(function() {
    'use strict';

    // Adjust the delay time (in milliseconds) as needed
    var delayTime = 5000; // 5 seconds

    // Hang the page by delaying the page load event
    window.addEventListener('load', function() {
        setTimeout(function() {
            console.log('Page hang complete');
        }, delayTime);
    });
})();
