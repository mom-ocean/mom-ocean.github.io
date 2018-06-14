## MOM Website Documentation

This is the source for the MOM5 documentation website

https://mom-ocean.github.io

The site is built using [Jekyll](https://jekyllrb.com/) and the [mimimal mistakes theme](https://mademistakes.com/work/minimal-mistakes-jekyll-theme/).

To be able to test the site locally (if you need to) you will need a working install of ruby and then install Jekyll and dependencies:

```sh
gem install bundler jekyll
```

and then to run the site locally to check your changes 

```sh
bundle exec jekyll serve
```

To push your changes back to the github repo
```sh
git commit -a -m "Commit message"
git push origin master
```
