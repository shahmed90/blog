# Blog Manual

## Local setup

- Clone repo
- Install `hugo` with `asdf` & leverage `.tool-versions`: Run `asdf install`
- Run `hugo serve -D` to fire up the web server incl. draft pages and access at [http://localhost:1313](http://localhost:1313)

## Write blogpost

- Create a new [page bundle](https://gohugo.io/content-management/page-bundles/) in `./content/posts` whereever you like. You can group posts in directories or dump everything in `posts`. Minimum requirement: New directory with an `index.md` and the [front matter](https://gohugo.io/content-management/front-matter/) with `title` and `date`
- Set `draft: true` to be able to commit stuff but don't publish it yet

## Write a generic page

- Same thing, but in `./content/pages` (theoretically wherever you like, but it's in the page URL)
- Add menu item in `config.toml`

## Deployment

Automated with GH Actions to GH Pages, don't break it! You might need to enable Pages initially, dunno if it will reset with ownership transfer.

## Updating the theme

Better ask, I did a manual change to the theme because it does not support subpaths as home.
