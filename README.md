void
====

void is a theme for Pelican. It's pretty much void of all color.
void uses an older version (1.2) of [Skeleton](http://www.getskeleton.com)
and [Font Awesome](http://fortawesome.github.io/Font-Awesome/).

Since I'm no designer, you should expect this to be a constant work in
progress.

You can see a live example of it [here](http://www.gregreda.com)

Screenshots
-----------
### Index
![Home Page](/examples/index.png)

### Article
![Article Page](/examples/article.png)

Example pelicanconf.py
----------------------
```python
#!/usr/bin/env python
# -*- coding: utf-8 -*- #

AUTHOR = u'Example Author Name'
SITENAME = u'Example Void Theme'
SITEURL = 'http://www.example.com'
TIMEZONE = 'America/Chicago'
THEME = 'void/'
AVATAR = '/theme/images/avatar.jpg'
TITLE = "Example: What is the title of your site?"
DESCRIPTION = "Lorem Ipsum something about your site and you too probably."

ARTICLE_URL = '{date:%Y}/{date:%m}/{date:%d}/{slug}/'
ARTICLE_SAVE_AS = '{date:%Y}/{date:%m}/{date:%d}/{slug}/index.html'

# Static Pages
PAGE_PATHS = ['pages']
PAGE_URL = '{slug}/'
PAGE_SAVE_AS = '{slug}/index.html'
ABOUT_PAGE_HEADER = 'Hello.'

# DEFAULTS
DEFAULT_LANG = 'en'
DEFAULT_CATEGORY = 'misc'
DEFAULT_DATE = 'fs'
DEFAULT_DATE_FORMAT = '%b %d, %Y'
DEFAULT_PAGINATION = False

# FEEDS
FEED_ALL_ATOM = "feeds/all.atom.xml"
TAG_FEED_ATOM = "feeds/tag/%s.atom.xml"

# PLUGINS
PLUGIN_PATHS = ['pelican-plugins', 'pelican_dynamic']
PLUGINS = ['assets', 'liquid_tags.notebook', 'pelican_dynamic', 'render_math']

CODE_DIR = 'code'
NOTEBOOK_DIR = 'notebooks'
EXTRA_HEADER = open('_nb_header.html').read().decode('utf-8')

STATIC_PATHS = ['images', 'code', 'notebooks', 'extra', 'data']
EXTRA_PATH_METADATA = {'extra/robots.txt': {'path': 'robots.txt'},}

NAVIGATION = [
    # You probably want to fill these in so they point to your user pages
    {'site': 'twitter', 'user': '', 'url': 'https://twitter.com/...'},
    {'site': 'github', 'user': '', 'url': 'https://github.com/...'},
    {'site': 'linkedin', 'user': '', 'url': 'http://linkedin.com/in/...'},
    {'site': 'google-plus', 'user': '', 'url': 'https://plus.google.com/...'},
    {'site': 'spotify', 'user': '', 'url': 'https://open.spotify.com/user/...'},
]

TWITTER_NAME = ""
TWITTER_CARDS = True
FACEBOOK_SHARE = True
HACKER_NEWS_SHARE = True

#### Analytics
GOOGLE_ANALYTICS = ''
DOMAIN = "example.com"

# Other
MAILCHIMP = False
CACHE_CONTENT = False
```
