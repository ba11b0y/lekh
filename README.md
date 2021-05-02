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

### Installing Hugo

```sh
# For Linux
sudo apt-get install hugo

# For Mac
brew install hugo

# Detailed instructions at https://gohugo.io/getting-started/installing#readout
```

### Creating a new site

```sh
hugo new site <site_name>
```

### Adding lekh as a theme

```sh
cd <site_name>
git init
git submodule add https://github.com/ba11b0y/lekh.git themes/lekh
echo theme = \"lekh\" >> config.toml

```

Here's Hugo's [official guide](https://gohugo.io/getting-started/quick-start/) for more details.


## Personalization

Hugo looks for a `config.toml` in the root of your site.
To personalize the theme, copy the default config shipped with the theme

`cp themes/lekh/exampleSite/config.toml config.toml`

And then customize accordingly.

Or simply copy the below config and customize accordingly.

```toml

baseURL = "https://example.com/"
languageCode = "en-us"
title = "Example Lekh Site"
theme = "lekh"

[params]
Name = "Agent Smith"
About = "We're not here because we're free. We're here because we're __not__ free. There's no escaping reason. No denying purpose. Because as we both know without purpose, we would not exist.<br/> Read more [here](https://matrix.fandom.com/wiki/Agent_Smith)"
Email = "agentsmith@thematrix.com"
Resume = "" # Add the filename with file extension.
PostLimit = 4 # Sets the number of posts to display on the front page
GoatCounterCode = ""

[[params.profiles]]
name = "GitHub"
url = "https://github.com/ba11b0y"

[[params.profiles]]
name = "Twitter"
url = "https://twitter.com/ba11b0y"

[[params.profiles]]
name = "Goodreads"
url = "https://www.goodreads.com/user/show/91520565-rahul-tiwari"

[[params.profiles]]
name = "LinkedIn"
url = ""

```

## Creating posts

```sh
# This creates a new draft post in content/posts
hugo new posts/title-of-post.md
```

## Serving it up

```sh
# This will show up your draft posts as well.
hugo server -D
#OR

#This will show up only your published posts.
hugo server
```

## Credits

* Thanks to [Vegard's](https://github.com/vegarsti) personal site from which the theme was heavily inspired.
* Also to https://www.gwern.net/ for the dark mode.

Feel free to contribute and open issues.
