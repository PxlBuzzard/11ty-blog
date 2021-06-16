---
layout: layouts/post.njk
title: Building the Danieljost.com Website
date: 2012-12-16
tags: website
---

Building a site to showcase yourself is hard. Even after working on websites professionally for three years I didn't have a grand vision in my head of what the site should look like. However I knew I that I was going to make it exactly the way I wanted it since I haven't had the luxury of complete creative control on a website since I started working professionally.

<em><strong>Preparations</strong></em>:

Before getting started I got my website hooked up with <a href="https://www.cloudflare.com">Cloudflare</a>. It does two awesome things: speeds up load times and keeps your site online even if your server goes down. To kick-start the design I found a great template called Responsive, as created using <a href="http://www.initializr.com/">Initializr</a>. It gave me a template for the CSS that makes the site scale appropriately to different screen sizes, which is a necessity in modern web design. I've included <a href="http://leaverou.github.com/prefixfree/">Prefix free</a> to simplify my CSS code and <a href="http://code.google.com/p/html5shiv/">HTML5Shiv</a> is used to ensure I can write HTML5 without worrying about compatibility in IE. I've added <a href="http://www.red-root.com/sandbox/holmes/">Holmes</a> for development to ensure I stick to proper design standards. Lastly I am using <a href="http://protofluid.com/" target="_blank">ProtoFluid</a> to view the site in different resolutions while maintaining my work setup on my computer. It's awesome.

<em><strong>The menu bar</strong></em>:

After seeing the fantastic menu bar built by <a href="http://amanita-design.net/" target="_blank">Amanita Design</a> I knew I wanted to use it. However they used <a href="http://jquery.com/" target="_blank">jQuery</a> coupled with a <a href="http://jquery.malsup.com/cycle/" target="_blank">Cycle</a> plugin and I wanted to see the same effect replicated using purely CSS. You can see a boiled-down version of the menu I built below (or at <a href="http://codepen.io/PxlBuzzard/pen/GbvKj" target="_blank">CodePen</a> if the embed is broken). The trick is to use text-shadow to duplicate the text, then increase the height the same amount that you decrease the margin-top, which effective makes the button look like it is scrolling up.
<pre class="codepen" data-height="300" data-type="result" data-href="GbvKj" data-user="PxlBuzzard" data-safe="true"><code></code></pre>
<script async src="http://codepen.io/assets/embed/ei.js"></script>

<strong>Multiple resolutions:</strong>

The entire time I was building the site I tweaked the CSS to ensure it would look good on any device. I want people looking to buy my web design services to see the site on their desktop in its full beauty, but I also need to be able to pull out my iPhone in a conference to quickly show a potential employer. With the rising prevalence of browsing on tablets I made the site looked great on my iPad as well.

<em><strong>Final Touches</strong></em>:

I added the menu from <a href="http://danieljost.com/">danieljost.com</a> to the blog that I assume you are reading this on to provide consistency across the site.

<strong>The future:</strong>

I haven't implemented everything I want yet. I would like to give each project its own page with some text, pictures, and maybe a video. My <a href="http://danieljost.com/resume" target="_blank">Resume</a> is lacking a good couple paragraphs describing myself and I want to have a true resume. However I am very pleased with what I have so far.
