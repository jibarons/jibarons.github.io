# Install ruby devkit

https://rubyinstaller.org/

# start command prompt with Ruby

` install jekyll bundler`

# Open Git bash and navigate to repository local dir

` cd ~/documents/repositories/.../username.github.io`

# cretae jekyll gem 

Cretes it in specifed directory

`jekyll new ~/documents/Repositories/jibarons.github.io/pages` 

creates it in current directory

`jekyll new .`

# For more follow

https://docs.github.com/en/pages/setting-up-a-github-pages-site-with-jekyll/creating-a-github-pages-site-with-jekyll

https://jekyllrb.com/

https://kbroman.org/simple_site/

point 9 and more...

# Test you site locally

Run in git bash, in publishing source directory `~/documents/Repositories/jibarons.github.io`

```
$ bundle exec jekyll serve
...
$ http://localhost:4000
```

# See theme layouts and files

in git command get  path  with:

`bundle info --path time-machine` time-machine = theme info


# Creating the site

Link to pages

`{% link _collection/name-of-document.md %}`
`[Link to a document]({% link _collection/name-of-document.md %}) # embeeded in .md` 

Link to post

`# {% post_url 2010-07-21-name-of-post %}`
`# {% post_url /subdir/2010-07-21-name-of-post %}`

Same as link to pages cna be embeeded in md


# Set a global permalink

To set a global permalink, you use the permalink variable in `_config.yml`. You can use placeholders to your desired output. For example:

`permalink: /:categories/:year/:month/:day/:title:output_ext`

Note that pages and collections (excluding posts and drafts) don’t have time and categories (for pages, the above `:title` is equivalent to `:basename`), these aspects of the permalink style are ignored for the output.

For example, a permalink style of `/:categories/:year/:month/:day/:title:output_ext` for the posts collection becomes `/:title.html` for pages and collections (excluding posts and drafts).


# Fix API authentication in jekyll to github
https://knightcodes.com/miscellaneous/2016/09/13/fix-github-metadata-error.html

add `github: [metadata]` to `_config.yml` 
https://github.com/github/pages-gem/issues/399