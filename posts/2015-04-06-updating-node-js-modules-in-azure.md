---
layout: layouts/post.njk
title: Updating a Node.js App in Azure

date: 2015-04-06
published: false
tags: [Web Development, node.js, Azure]
---

Recently I moved my [Ghost](https://ghost.org/) blog from [OpenShift](https://www.openshift.com/) to [Azure](http://azure.microsoft.com/en-us/). After following [some instructions](http://www.howtoinstallghost.com/how-to-install-ghost-on-windows-azure/) on how to install Ghost in Azure (it's easy), I was disappointed to see it was a couple versions behind the latest.

### Updating your app

In my case, I downloaded the latest version of Ghost from [Github](https://github.com/TryGhost/Ghost). I logged in via FTP and updated the files. I toyed with the idea of doing this via the console, but without an unzip command I figured FTP was the best route.

### Opening a console in Azure

Having a console is so much faster than moving `node_modules` over FTP. To get one, go to `https://<your-site-name>.scm.azurewebsites.net/` and open the `Debug Console`. Use `cd site/wwwroot` to get to your hosted content. In this directory, you should see at least see `package.json` if not a `node_modules` folder.

### Installing Node packages

From this point, you should make sure your website is stopped in the [Azure console](https://manage.windowsazure.com). If you do not stop the site, you will very likely run into errors with files already being in use.

From here, you have a couple options:

1. `npm update` is the standard method for updating an existing installation. Give it a try, and if it works then you're done. If not:
2. `rmdir node_modules /s /q` will delete the `node_modules` folder and give you a clean slate. `npm install` should work from here.

You can now start your site back up.
