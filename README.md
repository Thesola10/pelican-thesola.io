# My Pelican theme
A theme derived from Blue Penguin, liberally adapted into my graphical style.

## Features
Some features were added to articles to enhance reading experience.

The `Summary` metadata key will be shown instead of the shortened article body in article list pages.

The `Image` metadata key will show a thumbnail image next to the article in article list pages.

A left-aligned pull-quote can be created using the `<pullquote>` HTML tag, and made right-aligned by using `<pullquote right>`.

## Settings
```python
# Required! Currently valid archetypes: 'blog' or 'front'
ARCHETYPE = 'blog'

# all the following settings are *optional*

# HTML metadata
SITEDESCRIPTION = ''

# Use logo instead of site name
SITELOGO = '/images/logo.png'
SITELOGO_DARK = '/images/logo-dark.png'

# If set, article list will be replaced with the hidden page matching this slug
INDEX_SLUG = 'index'

# all defaults to True.
DISPLAY_HEADER = True
DISPLAY_FOOTER = True
DISPLAY_HOME   = True
DISPLAY_MENU   = True

# provided as examples, they make ‘clean’ urls. used by MENU_INTERNAL_PAGES.
TAGS_URL           = 'tags'
TAGS_SAVE_AS       = 'tags/index.html'
AUTHORS_URL        = 'authors'
AUTHORS_SAVE_AS    = 'authors/index.html'
CATEGORIES_URL     = 'categories'
CATEGORIES_SAVE_AS = 'categories/index.html'
ARCHIVES_URL       = 'archives'
ARCHIVES_SAVE_AS   = 'archives/index.html'

# use those if you want pelican standard pages to appear in your menu
MENU_INTERNAL_PAGES = (
    ('Tags', TAGS_URL, TAGS_SAVE_AS),
    ('Authors', AUTHORS_URL, AUTHORS_SAVE_AS),
    ('Categories', CATEGORIES_URL, CATEGORIES_SAVE_AS),
    ('Archives', ARCHIVES_URL, ARCHIVES_SAVE_AS),
)
# additional menu items
MENUITEMS = (
    ('GitHub', 'https://github.com/'),
    ('Linux Kernel', 'https://www.kernel.org/'),
)

# example pagination pattern
PAGINATION_PATTERNS = (
    (1, '{url}', '{save_as}'),
    (2, '{base_name}/page/{number}/', '{base_name}/page/{number}/index.html'),
)

```

## Contributors
See [CONTRIBUTORS.md](CONTRIBUTORS.md).
