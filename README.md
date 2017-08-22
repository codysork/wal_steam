# wal_steam

A little script that themes the colors for Metro for steam from wal or wpg.

## About

[Wal](https://github.com/dylanaraps/pywal) is a little program for linux that creates a terminal color scheme based on your wallpaper (in addition to being able to set the wallpaper and a few other 
interesting features).

[Wpgtk](https://github.com/deviantfero/wpgtk) is based on wal, but with the added feature of being able to generate gtk themes with the colors and bring a nice simple ui to wal.

Wal Steam is a tiny program that is meant to work with either of them, by reading the colors they generate and making a color theme for a slightly tweaked version of Metro for Steam.

[Metro for steam](http://metroforsteam.com/) is a very nice looking skin for steam. We also add the [community patch](https://steamcommunity.com/groups/metroforsteam/discussions/0/527273789693410879/) which makes the skin render well on linux.

## Install

The install is very simple and if you run into any problems just submit an issue and we should be able to resolve it fairly quickly.

First install wal or wpgtk (I'd suggest wpgtk since it will theme gtk too)

Then install steam using your distros package manager. (On ubuntu you need to enable the multiverse and fedora you'll want to get rpm fusion)

Next simply clone the repo to a memorable location like documents.

`git clone https://github.com/kotajacob/wal_steam.git ~/Documents`

That's it, the first time you run wal steam it will download all the needed skins and patches and apply them.

## Using

First cd into the wal_steam directory. Then you can just run the script with python. Use -g for wpg or -w for wal.

Example:

`python wal_steam.py -g`

```
Usage:
  wal_steam.py (-w | -g)
  wal_steam.py (-h | --help)
  wal_steam.py (-v | --version)

Options:
  -w                   use wal for colors
  -g                   use wpg for colors
  -h --help            show this help message and exit
  -v --version         show version and exit
```