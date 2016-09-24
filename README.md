# Webjeda Slides
Webjeda slides is built using revealjs. The idea is to keep all the slideshows in one place as posts. All your presentations can be accessed from one place!


# Features

## All the presentations at one place!
This theme is useful for those who give speeches at conferences using slides, students and teachers. Manage all your presentations at one place!

## Light-weight
The theme has very less code and uses minified assets for fast loading.

# Installation
Fork the ``master`` branch and delete ``gh-pages`` branch in it. This is important because ``gh-pages`` branch is used here only to host the blog. You should be using the master branch as the source and create a fresh ``gh-pages`` branch.

## How to delete old **gh-pages** branch?
After forking the repository, click on **branches**.


![delete gh-pages branch](/images/delete-github-branch.png)

Delete ``gh-pages`` branch.
![delete gh-pages branch](/images/delete-github-branch-2.png)

You have to create a new ``gh-pages`` branch using the master branch. Go back to the forked repository and create ``gh-pages`` branch.

![create gh-pages branch](/images/create-gh-pages-branch.JPG)

Now, go to settings and check the **Github Pages** section. You should see a URL where the blog is hosted.

This process will host the theme as a **Project Page**. You can also download the files for local development. 

Default theme will look like this

![webjeda slides jekyll theme](/images/slide-jekyll-theme.png)

This theme is responsive.

![webjeda slide responsive jekyll theme](/images/slide-responsive-jekyll-theme.png)


# Customization

## Theme
Posts can have any theme among the ones listed below. Different posts can have different themes. Use these values in the front matter to change theme - **black, white, league, sky, beige, simple, serif, blood(default), night, moon, solarized**.

```
---
title: Presentation 1
layout: post
theme: white 
---
```

# Development
Make changes to the **master** branch and create a pull request. Do not use **gh-pages** branch as it is used to host the theme.

# License
Read [LICENSE](https://raw.githubusercontent.com/sharu725/slides/master/LICENSE.md)