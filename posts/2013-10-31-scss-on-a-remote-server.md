---
layout: layouts/post.njk
title: Using SASS on a remote server
date: 2013-10-31
tags: web development
---

Sass is a Ruby gem. This is not helpful when you use Python/Django for your site.

Finding no easy ways to do it in Python, I installed Ruby, rubygems, and compass (which has sass).

It might've ended here, but I wanted more efficiency and less complexity.

**The problem:** Sass 'watch' can keep an eye on a directory and compile the SCSS to a seperate folder. However, I also needed to push that CSS to the live site immediately in order to reflect changes (since I developed the site with production mode enabled).

**First solution:** Install [filewatcher](https://github.com/thomasfl/filewatcher) for Ruby, which can monitor a folder and run a command when a file is modified. I ended up crafting this mediocre command:

	filewatcher *.scss -l ./MAGIC/static/magic/scss/*.scss "echo -e '\e[0;36m\nAn SCSS file has been modified.\e[0m'
	&& sass --update ./MAGIC/static/magic/scss/:./MAGIC/static/magic/css
	&& cp -r ./MAGIC/static/magic/css/ ./static/magic/
	&& echo -e '\e[0;32mCSS folder successfully copied to static.\e[0m'"

Put that in a .sh file and you're good to go. Except...

**Limitation:** I couldn't make filewatcher recurse through directories.

**Second solution:** Kill Ruby, use [inotify-tools](https://github.com/rvoicilas/inotify-tools). This can recursively watch directories for file modifications and offer more powerful output. Also it's slightly more readable:

	CURPATH='(removed to protect the innocent)'

	inotifywait -mr --timefmt '%d/%m/%y %H:%M' --format '%T %w %f' \
	-e close_write,moved_to,create ./MAGIC/static/magic/scss/ | while read date time dir file; do

       FILECHANGE=${dir}${file}
       # convert absolute path to relative
       FILECHANGEREL=`echo "$FILECHANGE" | sed 's_'$CURPATH'/__'`

       echo -e "\e[0;36m\n${file} was modified.\e[0m"
       sass --update ./MAGIC/static/magic/scss/:./MAGIC/static/magic/css
       && cp -r ./MAGIC/static/magic/css/ ./static/magic/
       && echo -e "\e[0;32m${file} was compiled to CSS and copied to static.\e[0m"
	done

**The probably better solution:** Use [Grunt](http://gruntjs.com/). The downside here is that I need to run Node.js on the server, which is yet-another-language that adds complexity to the stack. For now inotify-tools gets the job done well.
