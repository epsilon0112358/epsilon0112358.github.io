---
created: 2025-04-29
---
# Blog setup

A couple of notes on how I setup the infrastructure around the page you are looking at.

# GitHub
This page is hosted on GitHub, specifically [GitHub pages](https://pages.github.com/). If you have an account there, all you need to do is create a respective repository.
If you don't have an account yet, you can sign up for free!

*For casual version control with Git I prefer to use a GUI, namely [SourceTree](https://www.sourcetreeapp.com/) over the command line*
# MkDocs
I already had Python installed on my computer, so I could jump right into the official [installation guide](https://www.mkdocs.org/user-guide/installation/).

One of the native themes is called Material, and not only is it already beautiful, there's also a wealth of documentation around it. I found the documentation from [squidfunk](https://squidfunk.github.io/mkdocs-material/setup/) tremendously helpful. (e.g. for different [color themes](https://squidfunk.github.io/mkdocs-material/setup/changing-the-colors/), the [blog](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/) architechture, or how to setup the [navigation](https://squidfunk.github.io/mkdocs-material/setup/setting-up-a-blog/) sidebar).
There are other beautiful themes out there, however they do not integrate with the native blog plugin as smoothly. Still fun to [take a look](https://pawamoy.github.io/mkdocs-gallery/) though!

By Default, MkDocs renders the markdown files into a subdirectory /sites.
If you don't care for the original files and just want the GitHub pages to show the HTML part, you could make this subdirectory the repository.
I opted to keep the entire root directory including markdown and all in one repository, and host the GitHub pages *from that subdirectory*, [like so](https://stackoverflow.com/a/75662195).

Adding the "last updated" note on the bottom of each page here took some digging as well. I used [this feature](https://henrywhitaker3.github.io/mkdocs-material-dark-theme/plugins/revision-date/) for that.

# Obsidian
[Obsidian](https://obsidian.md/) is an all time favorite for note taking with markdown.
I simply made the main directory of my repository's local copy a vault, and edit the content from there!
I've always used plugins sparingly, trying to get as much out of the native functionality as possible. I do however recommend the [DataView](https://github.com/blacksmithgu/obsidian-dataview) community plugin for various query needs!