------------
Why use energize?

Touch devices sometimes add an artificial delay to click events, just to make sure the user isn't double-tapping to zoom.

Why not just bind to ontouchend?
-------------

Because the user might touch an element to scroll.  Do you want a click event to fire when the user was intending to scroll?


Why fire simulated touch events?  Why not just use something like <a href="http://code.google.com/mobile/articles/fast_buttons.html">Fast Button</a>?
-------------

Because you have to add click events to EVERYTHING you want to speed up.  Also, interaction with native form elements such as buttons aren't sped up unless you manually add events to them.  Energize listens for clicks bubbling up to the top and handles them appropriately so you don't have to worry about them.
