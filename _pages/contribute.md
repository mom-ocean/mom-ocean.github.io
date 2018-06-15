---
layout: single
permalink: /contribute/
author_profile: true
toc: true
---
## Introduction

The MOM5 source code, experimental configurations and documentation are published on [GitHub](https://github.com/mom-ocean/mom5) using a GPLv2 license. Users are very much encouraged to contribute code changes and improvements back to the main code repository. By doing this you are helping all users by building a better model. Please remember that every contribution is valueable no matter how small - whether it be changes to the documentation, improvements in code understandability or formatting, or a whole new algorithm.

## Using GitHub Pull Requests

MOM5 uses github 'pull requests' to facilitate code contributions from the community. Think of it as a request to the project maintainers to pull in or accept some code changes. Here we'll step through the process of making code changes, submitting a pull request and having it merged into the main repository.

### Step 1: make a github account

Go to [GitHub](https://github.com) and create an account. Github is a website that hosts software using the [git](http://mom-ocean.org/web/docs/git) Version Control System (VCS). It is free to use for public repositories.

### Step 2: make an issue to describe your changes

Go to the [MOM5 GitHub page](https://github.com/BreakawayLabs/mom) and click on the 'issues' tab at the top of the page and then the 'New issue' button on the right hand side. Log your issue and take note of the issue number.

### Step 3: fork MOM5 and download your new repository

Once you've logged in to GitHub go to the [MOM5 GitHub page](https://github.com/BreakawayLabs/mom) and click on 'fork' in the top right hand corner of the page. [This image](http://hisham.hm/img/posts/github-fork.png) from [Hisham's blog](http://hisham.hm/2016/01/01/how-to-make-a-pull-request-on-github-a-quick-tutorial/) shows the button location.

This will create your own independent copy of the MOM5 repository within your GitHub account. Now it's time to download the new repository and make some changes. To download the repository open a shell/terminal and type:

```sh
$ git clone git@github.com:<your github user name>/mom.git
```

### Step 4: create a branch, make your code changes and commit them

Once you've download the MOM5 source code in the form of a git repository it's time create a branch. This is place to hold a collection of more or less independent code changes. In your terminal:

```sh
$ cd mom
$ git checkout -b <new_branch_name>
```

Now make your code changes to any files. In order to commit these changes to your branch:

```sh
$ git commit -a -m "<commit message #<issue number>"
```

Note that the commit message includes the issue number preceded by the '#' character. This allows individual commits to be linked to their issues.

### Step 5: push changes back to your fork

After you've committed working changes you'll want to push them back to your fork on GitHub.

```sh
$ git push origin <new_branch_name>
```

Your changes should now be visible on your MOM5 fork GitHub page.

### Step 6: make the pull request

This is the last step! Once you've pushed the code changes go to the GitHub page for your MOM5 for and you should see a button "compare & pull request". Click on this, review your additions/changes and then click on the confirm button. Once again [this image](http://hisham.hm/img/posts/github-comparepr.png) shows the location of the button.

## Getting Help

If you have changes that you would like to contribute to MOM5 but are not comfortable creating a pull request as described about please don't give up. Write an email to the [MOM5 mailing list](https://groups.google.com/forum/#!forum/mom-users) and someone will help.

## Useful Links

* [Hisham's pull request tutorial](http://hisham.hm/2016/01/01/how-to-make-a-pull-request-on-github-a-quick-tutorial/)
* [GitHub documentation of forking](https://help.github.com/articles/fork-a-repo/)
* [GitHub documentation on pull requests](https://help.github.com/articles/creating-a-pull-request/)
* [GitHub documentation on code collaboration](https://help.github.com/categories/collaborating-on-projects-using-issues-and-pull-requests/)
* [Other git links](http://mom-ocean.org/web/docs/git)
