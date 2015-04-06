BeatMaster
==========

Minimal framework for when your DOM/UI/application performance is of utmost importance: it provides an 'animationFrame'-driven state machine to help you sequence, schedule and manage your application tasks. 

Use BeatMaster when MVC/MVP sounds nice but doesn't cut it helping you stay in control of your application and you want to be able to optimize it without losing your mind. BeatMaster will drive your slaves. 

Use BeatMaster when you feel your app can benefit from the characteristics of a 'game engine' while maybe not being a game itself.

---

Related Efforts
---------------

- Throttling user inputs ( http://spoike.ghost.io/user-input-framerate-throttling-in-the-browser/ )

  Here the idea is to throttle user input events, discarding the ones that come in too fast. A naive use of this will destroy user 'control' of the application: you will need to do something about it by aggregating or otherwise tracking the user inputs you'ld destroy/skip. It is related to the *BeatMaster* concept as it is another design to fundamentally improve performance of in-browser application through *throttling*. *BeatMaster* does so by throttling the browser repaint activity directly; this one does so by attempting the same *indirectly*, as handling fewer user inputs would result in fewer UI updates and thus fewer browser repaint jobs:

  + http://www.html5rocks.com/en/tutorials/speed/unnecessary-paints/   
  + http://www.html5rocks.com/en/tutorials/internals/howbrowserswork/
  + https://developers.google.com/speed/articles/reflow
  + http://stackoverflow.com/questions/2549296/whats-the-difference-between-reflow-and-repaint
  + http://www.stubbornella.org/content/2009/03/27/reflows-repaints-css-performance-making-your-javascript-slow/
  + http://csstriggers.com/ & http://aerotwist.com/blog/css-triggers/
