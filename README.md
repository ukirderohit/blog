# blog
Simple jekyll blog

[Demo](http://www.ukirderohit.me/blog)

![blog screenshot](http://www.ukirderohit.me/blog/images/blog.JPG)

This is a simple, beautiful theme for Jekyll that emphasizes content rather than aesthetic fluff. It's mobile _first_, fluidly responsive, and delightfully lightweight.

It's pretty minimal, but leverages large type and drastic contrast to make a statement, on all devices.


## Getting Started

> :warning:
  This requires ruby and rubygems installed :-

* [x] Clean layout
* [x] Resposive layout
* [x] Preprocessor SASS
* [x] HTML minified
* [x] CSS minified
* [x] No Javascript
* [x] Pagination
* [x] Syntax highlight
* [x] Author config
* [x] Comments with Disqus
* [x] Share posts

---

If you're completely new to Jekyll, I recommend checking out the documentation at <http://jekyllrb.com>.


### Fork, then clone

Fork the repo, and then clone it so you've got the code locally.

```
$ Fork or clone repo `git clone git@github.com:ukirderohit/blog.git`
$ cd blog
$ gem install bundler # If you don't have bundler installed
$ bundle install
$ Start Jekyll server: `jekyll serve`
```

Access, [localhost:4000/simplest](http://localhost:4000/blog)


### Modify the `_config.yml`

The `_config.yml` located in the root of the Pixyll directory contains all of the configuration details
for the Jekyll site. The defaults are:

```yml
# Site settings
title: Rohit Ukirde
email: your_email@example.com
author: Rohit Ukirde
description: "A simple, beautiful theme for Jekyll that emphasizes content rather than aesthetic fluff."
baseurl: ""
url: "http://ukirderohit.me"

# Build settings
markdown: kramdown
permalink: pretty
paginate: 4
```

### Jekyll Serve

Then, start the Jekyll Server. I always like to give the `--watch` option so it updates the generated HTML when I make changes.

```
$ jekyll serve --watch
```

Now you can navigate to `localhost:4000` in your browser to see the site.


### Using Github Pages

You can host your Jekyll site for free with Github Pages. [Click here](https://pages.github.com/) for more information.


#### A configuration tweak if you're using a gh-pages sub-folder

In addition to your github-username.github.io repo that maps to the root url, you can serve up sites by using a gh-pages branch for other repos so they're available at github-username.github.io/repo-name.

This will require you to modify the `_config.yml` like so:

```yml
# Site settings
title: Repo Name
email: your_email@example.com
author: Rohit Ukirde
description: "Repo description"
baseurl: "/repo-name"
url: "http://github-username.github.io"

# Build settings
markdown: kramdown
permalink: pretty
paginate: 4
```

This will ensure that the the correct relative path is constructed for your assets and posts. Also, in order to run the project locally, you will need to specify the blank string for the baseurl: `$ jekyll serve --baseurl ''`.


## Thanks to the following

* [Jekyll](http://jekyllrb.com)


## Contributing

1. Fork it
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create new Pull Request

## How to use this theme

Fork the ``master`` branch and delete ``gh-pages`` branch in it. This is important because ``gh-pages`` branch is used here only to host the blog. You should be using the master branch as the source and create a fresh ``gh-pages`` branch.


## How to delete old **gh-pages** branch?
After forking the repository, click on **branches**.

![delete gh-pages branch](http://ukirderohit.me/blog/images/1.JPG)

Delete ``gh-pages`` branch.
![delete gh-pages branch](http://ukirderohit.me/blog/images/2.JPG)

You have to create a new ``gh-pages`` branch using the master branch. Go back to the forked repository and create ``gh-pages`` branch.

![create gh-pages branch](http://ukirderohit.me/blog/images/3.JPG)

Now, go to settings and check the **Github Pages** section. You should see a URL where the blog is hosted. If not select a branch as source.

### Copyright and license

It is under [the MIT license](/LICENSE).

Enjoy :yum:

