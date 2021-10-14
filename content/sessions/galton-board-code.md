+++
title = "Galton board code"
date = "2019-10-21T13:25:33+01:00"
authors = ["Ryan Moodie"]
cover = "img/galton-snap.png"
tags = ["outreach", "galton-board", "python", "raspberry-pi", "matplotlib", "numpy"]
description = "Ideas for improving the Galton board software"
showFullContent = false
type = "posts"
+++

##### Ideas for improving the Galton board software

* Mass of balls
* Size of balls
* Size of pins
* Width of barriers
* Fix lag
	* Due to N=300?
* Deploy on Pis from GitHub repo, automate updates
* Get light gates working
* Somehow show effect of large N
	* If performance is an issue, pre-calculate
* Add option to drip feed balls into simulation
* Check dependencies
* Add sliders to change physical parameters
* Change gravity on the fly? As a vector? Accelerometers in Pis?
* Maybe: allow barriers to be drawn in by hand
* Consider using some more up-to-date libraries? Touch screen interactivity, GUI, physics?
* Make it into a webapp? (not to replace Pi software, to provide in addition)

##### Plan of action 

* I've added the more pedestrian suggestions as [issues on the repo](https://github.com/eidoom/GaltonBoard/issues).
* We can assign people interested in working on these there.
