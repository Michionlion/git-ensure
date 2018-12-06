# git-ensure
A Small Utility to Ensure Git Repositories are Current


## Development
Edit `ensure.c` and build with `make` or `make ensure`.
Use `make run` or `./ensure` to run the executable.

### Example Output
```
--- Processing ./projects/comp/chapters ---
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
Already up to date.

--- Processing ./projects/saejinmh.com ---
On branch master
Your branch is up to date with 'origin/master'.

nothing to commit, working tree clean
remote: Enumerating objects: 60, done.
remote: Counting objects: 100% (55/55), done.
remote: Compressing objects: 100% (26/26), done.
remote: Total 44 (delta 12), reused 44 (delta 12), pack-reused 0
Unpacking objects: 100% (44/44), done.
From github.com:Michionlion/saejinmh.com
   ad17887..4f1c079  master     -> origin/master
Updating ad17887..4f1c079
Fast-forward
 content/_index.md                                  |   4 +-
 content/projects/thegallery/index.md               |  22 +++
 layouts/shortcodes/figure.html                     |  29 ++++
 layouts/shortcodes/gallery.html                    |  41 ++++++
 layouts/shortcodes/load-photoswipe.html            |  71 +++++++++
 static/css/hugo-easy-gallery.css                   | 159 +++++++++++++++++++++
 static/images/thegallery/creation/.gitkeep         |   0
 static/images/thegallery/users/an installation.jpg | Bin 0 -> 341051 bytes
 static/images/thegallery/users/look at that!.jpg   | Bin 0 -> 320051 bytes
 static/images/thegallery/users/oh, a portal!.jpg   | Bin 0 -> 264298 bytes
 .../images/thegallery/users/see it and feel it.jpg | Bin 0 -> 202237 bytes
 .../images/thegallery/users/that's a portal!.jpg   | Bin 0 -> 225740 bytes
 .../thegallery/users/very interesting wall.jpg     | Bin 0 -> 324899 bytes
 static/js/load-photoswipe.js                       |  80 +++++++++++
 14 files changed, 404 insertions(+), 2 deletions(-)
 create mode 100644 content/projects/thegallery/index.md
 create mode 100644 layouts/shortcodes/figure.html
 create mode 100644 layouts/shortcodes/gallery.html
 create mode 100644 layouts/shortcodes/load-photoswipe.html
 create mode 100644 static/css/hugo-easy-gallery.css
 create mode 100644 static/images/thegallery/creation/.gitkeep
 create mode 100644 static/images/thegallery/users/an installation.jpg
 create mode 100644 static/images/thegallery/users/look at that!.jpg
 create mode 100644 static/images/thegallery/users/oh, a portal!.jpg
 create mode 100644 static/images/thegallery/users/see it and feel it.jpg
 create mode 100644 static/images/thegallery/users/that's a portal!.jpg
 create mode 100644 static/images/thegallery/users/very interesting wall.jpg
 create mode 100644 static/js/load-photoswipe.js

```
