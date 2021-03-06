<h1 align="center">SoftyRoll</h1>
<p align="center">Just call the script (TTY or not) and stream it with webtorrent, dead simple!</p>

## In the terminal
<p align="center">
<img src="./TTY.gif" alt="Video Preview" width="600px">
</p>

## Outside the terminal
<p align="center">
<img src="./noTTY.gif" alt="Video Preview" width="600px">
</p>

### How does this work?

This is a shell script. It scrapes `nyaa.si` and gets the magnet link.
After this it uses [webtorrent](https://webtorrent.io/) to stream the video from the magnet link.
For scraping, the script uses simple gnu utils like sed, pr, cut.

## Features 

+ Cacheless
+ Works both in and outside the terminal
+ Realy simple 
+ Sorted by highest Seeder
+ POSIX shell only

## Requirements

* [webtorrent](https://webtorrent.io/) - A tool to stream torrent. `npm install webtorrent-cli -g`

## Installation

### cURL
cURL **SoftyRoll** to your **$PATH** and give execute permissions.

```sh
$ curl -sL "https://raw.githubusercontent.com/LamprosPitsillos/SoftyRoll/main/SoftyRoll" -o ~/.local/bin/SoftyRoll
$ chmod +x ~/.local/bin/SoftyRoll
```
- To update, just do `curl` again, no need to `chmod` anymore.
- To uninstall, simply remove `SoftyRoll` from your **$PATH**, for example `rm -f ~/.local/bin/SoftyRoll`.

## Credit 
This was heavily inspired by [Bugswriter/notflix](https://github.com/Bugswriter/notflix/blob/master/README.md).
The README is basically a copy from his project.
