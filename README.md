# jekyll-wgdd theme with multi language support

I'm trying to create a Jekyll theme which includes support for multiple
languages. Although I really like the minimal-mistakes theme it relies
on a site-wide defined locale to localize its UI. This makes it impossible to
use it for a site in different languages.

My idea here is simple: build all pages/posts from one Jekyll site and put them
into a language specific path, e.g.

/de/...
/en/...
/it/...

Posts should link to translated versions. I think about YAML fron matter like

translation:
  - lang: en
    post: '/en/_posts/XXXX-XX-XX-title.md'
  - lang: de
    post: '/de/_posts/XXXX-XX-XX-title.md'

Also menus and site titles/descriptions/... must be translateable.

<!-- vim: set tw=79 ts=2 sw=2 ai si et: -->
