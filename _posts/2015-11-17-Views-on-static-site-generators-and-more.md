---
layout: post
title:  "What about static sites, pre-compiled css and much more?"
date:   2015-11-17 13:18:55
categories: 1DV022
---

#### What do you think of pre-compiling your CSS?
  * Compare to regular CSS
  * Which techniques did you use?
  * Pros and cons?
   
I think that preprocessing CSS is a better way too structure and maintain your CSS-code with partials. Partials is CSS-files containing parts of your CSS-code and can be included into other CSS-files.
   
[Sass](http://sass-lang.com/) is the CSS prepropressor I used to style this site. It allows you to use variables, where you can save for an example color codes and reuse the variable where you want that color.
Sass also provides the ability to use mathematical operators to calculate width, height and  much more.

There are a lot of pros and some cons with preprocessed CSS, but here are some of them.

Pros:

* Variables
* Mixins, like functions
* Partials
* Nesting, makes it possible to have the same visual hierarchy as in HTML documents
* Mathematical operators 

Cons:

* Could be more difficult than regular CSS
* Needs more tools to setup and execute than regular CSS
* Takes more time
* Line numbers in your SASS files are not the same as final CSS file, there are ways to fiz this problem.

---

#### What do you think of static site generators?
  * What type of projects are they suitable for?
  
Static site generators are good for create simple sites where you want to present a minor amount of information without any database. For example blogs, presentation of a project or an static site for your sports club.
The SSG takes templates, text, html and makes a static site. I used Jekyll as a SSG, which is supported on GitHub pages.
Jekyll is a powerful tool which allows the user to make partials. Partials are parts of your html, for example head, header and footer, which you include to your default html-file.
This SSG helps you a lot with building an website, by creating layouts with html and Liquid templates. By using YAML front matter in the top of a markdown-file or a html-file Jekyll treats that file special and convert it into a correct html.file presented on the site.

Static site generators are smooth and really smart if you want to create a small website. If you feel the need to have use databases, admin UI, user input or realtime content you can't use SSGs.
You have to choose another method to build your site, because these static site generators only creates static content. Using SSGs are more complex than without, it requires more tools and also a hosting server which supports any your static site generator.

I found using Jekyll sometimes difficult. It took a lot of time too figure out how it was working, also how the "new" features worked.

---
  
#### What is robots.txt and how have you configure it for your site?

Robots.txt is for search-robots on the internet. Within robots.txt you configure what these robots are allowed to search for.
I configured it to disallow all robots to search for my site, because I don't have relative information which I want to expose for the robots.
It's not 100% sure no robots will visit and search through your site when configuring robots.txt to disallow robots. There are some bad robots out there which will ignore anything in robots.txt. 

---

#### What is humans.txt and how have you configure it for your site?

it's for humans to find information about who the website was created by and sometimes when. I configures it with my name and with a link to my github account.

---

#### How did you implements comments to blog posts

I use the service [Disqus](https://disqus.com/) provides for members to add their commenting window into my posts.
It's a window with javascript under the posts.

---

#### What is Open Graph and how do you make use of it?

Open Graph is implemented in the head to make it possible for websites such as facebook get a small amount of information about your site to display when people linking the site.
The information is depending on what you write in your sites head. I used Open Graph meta tags in my head.html, og tags with title, type, url and image. 
