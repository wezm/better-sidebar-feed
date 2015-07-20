Better Sidebar Feed
===================

A script that... you guessed it, generates a better RSS feed for
[Sidebar](http://sidebar.io/) (The 5 best design links, every day). Subscribe
to it at: [http://files.wezm.net/sidebar.xml](http://files.wezm.net/sidebar.xml).

Why is it better?
-----------------

* Icon & URL of linked article are shown.
* A brief description of article is included in entries (when available).

Installation/generation notes
-----------------------------

(Mostly for my own documentation)

```shell
bundle install --path vendor/bundle
```

```crontab
0 0,12 * * * cd /home/wmoore/better-sidebar-feed && bundle exec ./better-sidebar-feed > sidebar.xml && mv sidebar.xml /var/www/files.wezm.net/sidebar.xml
```
