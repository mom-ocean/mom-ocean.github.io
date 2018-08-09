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

# Layout

The site layout is rather simple:

```
|-- README.md
|-- _config.yml
|-- _data
|   `-- navigation.yml
|-- _docs
|   |-- 01-quickstart.md
|   `-- 02-user_guide.md
|-- _pages
|   |-- contribute.md
|   |-- docs.md
|   |-- home.md
|   `-- posts.md
|-- _posts
|   |-- 2015-11-28-stunning-so-viz.md
|   `-- 2018-06-14-new-history-of-mom.md
`-- assets
    |-- images
    |   `-- water.jpg
    `-- pdfs
        |-- Cox_1984_GFDL_Tech_Report_1.pdf
        |-- MOM1_READ_ME.pdf
        |-- MOM1_manual.pdf
        |-- MOM2_manual.pdf
        |-- MOM3_manual.pdf
        |-- MOM4_manual.pdf
        |-- MOM4p1_manual.pdf
        |-- MOM5_elements.pdf
        |-- MOM5_manual.pdf
        |-- mom_history_2017.09.19.pdf
        |-- mom_history_v15.09.05.pdf
        |-- testcase_ICCM.pdf
        |-- testcase_atl_regional.pdf
        |-- testcase_baltic.pdf
        |-- testcase_ocean_cpld.pdf
        `-- testcase_ocean_solo.pdf
```

All static material like images and pdfs go in the `assets` folder.

All top level pages (`home`, `docs`, `posts` and `contribute`) live in the `_pages` directory. 

New posts produce a new markdown file in the `_posts` directory with the date in the filename.

Documentation for how to use this theme and customise it is available here:

https://mmistakes.github.io/minimal-mistakes/docs/configuration/
