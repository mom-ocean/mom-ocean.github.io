---
layout: single
permalink: /downloads/
author_profile: true
toc: true
title: "Downloads"
sidebar:
    nav: "quicklinks"
---

MOM uses [git](http://git-scm.com/) for version control of all source code, documentation and data. A central repository is hosted on [GitHub](https://github.com/mom-ocean).

## Source code

The recommended method for accessing the source code is to use git to make a clone of the [repository](https://github.com/mom-ocean/MOM5). This will allow you to easily contribute any changes back to the MOM community.

### Users and Developers

It is recommended that MOM users and developers download the most recent code using the following command

```
git clone https://github.com/mom-ocean/MOM5.git
```

## Data

The complete distribution of MOM includes some large data files used for testing and examples. To save your bandwidth and keep source code checkouts fast, the data files are managed in a slightly different way to source code files.

All of the data files are hosted [here](http://portal.sf.utas.edu.au/thredds/catalog/momtest/catalog.html) by the [ARC Centre of Excellence for Climate Extremes](https://climateextremes.org.au) on services provided by the [Tasmanian Partnership for Advanced Computing](https://www.tpac.org.au).

The files can be downloaded manually into the `data/archives` directory or using a helper script:
```
./data/get_exp_data.py 
```
However, the preferred method is to download the necessary input data automatically when running a test case, for example:
```
./MOM_run --platform PLATFORM_ID --type MODEL_TYPE --experiment TEST_CASE --download_input_data
```