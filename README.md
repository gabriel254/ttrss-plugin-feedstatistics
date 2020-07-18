ttrss-plugin-feedstatistics
===========================

Basic feed statistics for Tiny Tiny RSS. 

Adds a statistics pane to the feed preferences tab, including both a Google Reader-style one line summary and a table of statistics per feed.

Notes
-----

1) The table is sorted by posts/day. No way to change this in the preferences, but you can easily change it in the SQL query.

2) We do not keep track of actual feed activity, but instead only look at the current database. This has a few implications, e.g. we do not keep lifetime read counts. 

3) The items per day calculation assumes all feeds were followed for the entire interval. If they were recently added, the value will be wrong.

Installation
------------

1) Clone the repository into [TT-RSS root directory]/plugins.local/feedstatistics

2) Set the correct permissions, if neeeded

3) Enable the plugin by going to Preferences -> Plugins

Thanks
---------

@aaronaxvig for adding all-item statistics.

Links
-----

For discussion, please see the following thread in the Tiny Tiny RSS forums.

https://community.tt-rss.org/t/add-feature-statistics/3242/6
