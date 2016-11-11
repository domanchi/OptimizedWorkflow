# devtools
> **When should you automate something?**

> A good rule of thumb is when you find yourself doing a task manually *twice*, write a tool to automate it *for the third time*.

This is a collection of tools that I use to become more effective in my job. Though mainly for personal use,
please feel free to borrow, edit or improve my scripts to tailor it to your own workflow.

### Layout
#### /configs
These configuration files are abridged saved copies of keyboard shortcuts and preferences I use for my favorite applications.

#### /scripts
These are bash scripts that automate certain manual tasks that I find myself doing over and over again. Previously, these
existed as a random assortment of local scripts; however, after being inspired by the following quote, I decided to invest
a little bit more time in maintaining my toolset, with the goal of being able to move into a new environment, clone this repo,
and get right down to business.

A recent addition to this tooling set is the ability to modularize bash scripts with **namespaces**. Simple, clean, manageable
code is good code, so I designed an interface which allows me to divide my scripts into sensible chunks, and import them
as needed. For more information, see [/scripts/main.sh] (https://github.com/domanchi/devtools/blob/master/scripts/main.sh).

### Installation
#### /configs
Just override your existing config files with these ones. 'nuf said.

#### /scripts
Within your `~/.bash_profile`, include the following line:
```
# This will import all functionality from devtools.
. /path/to/devtools/scripts/main.sh
```

You may need to `chmod +x scripts/main.sh` in order to make it work. Also, you can configure the features/functionality you
want within main.sh.
