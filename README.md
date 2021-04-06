# Lekh
Simple, text-focussed and minimal personal portfolio theme based on https://github.com/vegarsti/vegarsti.github.io

## Screenshot ([Live Demo](https://agitated-yonath-d9c445.netlify.com/))
![Screenshot](https://raw.githubusercontent.com/invinciblycool/lekh/master/images/screenshot.png)

## Features
* Social media links
* Markdown supported
* Easy to personalize
* RSS feed
* Dark mode (taken from https://www.gwern.net/ as it is.)
* GoatCounter counts(analytics). Know more about GoatCounter [here](https://goatcounter.com)


## Installation

cd into your hugo site's root directory and:

```sh
cd themes
git clone https://github.com/invinciblycool/lekh.git
```

For more information read the [official setup guide](https://gohugo.io/overview/installing/) of Hugo.


## Personalization

To personalize the theme

`cp themes/lekh/exampleSite/config.toml config.toml`

And then customize accordingly.

Or simply copy the below config and customize accordingly.

```toml

baseURL = "http://rtiwari.me/"
languageCode = "en-us"
title = "Rahul Tiwari"
theme = "lekh"

[params]
Name = ""
Email = ""
Resume = "" # Add the filename with file extension.
PostLimit = 4 # Sets the number of posts to display on the front page
GoatCounterCode = ""

[[params.profiles]]
name = "GitHub"
url = ""

[[profiles]]
name = "Twitter"
url = ""

[[params.profiles]]
name = "Goodreads"
url = ""

[[params.profiles]]
name = "LinkedIn"
url = ""

```

## Posts

Below is a typical post, which defaults to what Hugo expects.

Specify `draft: true` to avoid publishing the post.

```md
---
title: "Rant post"
date: "2020-04-02"
draft: true
---

Too much to rant :(
```

## Credits

* Thanks to [Vegard's](https://github.com/vegarsti) personal site from which the theme was heavily inspired.
* Also to https://www.gwern.net/ for the dark mode.

Feel free to contribute and open issues.
