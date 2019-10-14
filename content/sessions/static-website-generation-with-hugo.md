+++
title = "Static website generation with Hugo"
date = "2019-10-14T16:55:21+01:00"
author = "Ryan Moodie"
cover = "img/hugo-logo-wide.svg"
tags = ["websites"]
description = ""
showFullContent = false
type = "posts"
+++

Today I unveiled our new website! Thanks to Daniel for hosting. It's powered by Hugo, a static website generator. 

The best way to install (the latest version of) Hugo can be found [here](//gohugo.io/getting-started/installing/#binary-cross-platform). In short, download the latest [release](//github.com/gohugoio/hugo/releases) and add the binary to your path.



Here's how you can add your sessions to the site:

* Speak to me if you don't already have write permissions

* clone the [repo](https://github.com/eidoom/computing-club-site): 
```shell
git clone git@github.com:eidoom/computing-club-site.git
```

* navigate to the root directory of the repo locally
```shell
cd computing-club-site
```

* pull the theme by running 
```shell
git submodule update --init --recursive --remote
```

* make your new session page by running 
```shell
hugo new sessions/NAME.md
```

* edit the metadata within the `+++`'s and write the body of your page in markdown at the bottom of the file
```shell
vim content/sessions/NAME.md
```
The metadata field `cover` should point at the cover image for your page. Add the image file to `static/img` along with any other images (or other media files) you include

* stage your changes
	* If you want to push the newly compiled website, first generate the updated static website by running
	```shell
	hugo
	```
	then
	```shell
	git add .
	```
	* If you want to push your changes to the source without pushing the compiled website, just
	```shell
	git add content/sessions/NAME.md static/img/PHOTO.png
	```
	and any other media files you included

* then finally push your changes to the remote repo 
```shell
git commit -m "MESSAGE"
git push
```
and you're done!

Have a look at the [source for this page](//github.com/eidoom/computing-club-site/blob/master/content/sessions/static-website-generation-with-hugo.md) if you like. The [Hugo docs](//gohugo.io/categories/getting-started) are also pretty good.
