# Development

This project is 99% code from [PlaceNL/Bot](https://github.com/PlaceNL/Bot/)

## Collaboration

We are in the [fuckcars discord](https://discord.com/channels/959481781202059284/959810250146459668).

## Merging PlaceNL changes

* Add their repo as a remote called "upstream":
	```
	git remote add upstream https://github.com/PlaceNL/Bot.git
	```
* Fetch their changes and merge them
	```
	git fetch upstream
	git merge upstream/master
	```
* If needed: Fix merge conflicts and commit them
	```
	git add ....
	git merge --continue
	```

## Main differences to PlaceNL/Bot:

* Our command server is `placefc.herokuapp.com`. The URL is in multiple places.
* UserScript headers in `fuckcarsbot.user.js`: `@name`, `@namespace`, `@description`, `@author` and `@connect` are changed.
* Strings in `fuckcarsbot.user.js` are translated to english.
* We don't build the docker image, so the instructions for docker are removed. If you have time, you can look into that.
