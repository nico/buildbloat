buildbloat
==========

Converts [ninja](http://martine.github.io/ninja/) build logs to
[webtreemap](https://github.com/martine/webtreemap) json files.

Run `ninja -t recompact` first ot make sure that no duplicate entries are
in the build log, and use a ninja newer than 1.4 to make sure recompaction
removes old, stale buildlog entries.

Usage:

    buildbloat.py out/Release/.ninja_log > data.json
