# GH Pages Site (Minimal Jekyll)
Website template for a Markdown-based docs site hosted on GH Pages

## **Features**

- Suitable for light docs site of a few pages.
- No HTML or Liquid coding needed. Just write content in markdown.
- No coding experience need to setup or work on.
- No Jekyll config, theme or packages to install.
- Uses a default minimal theme provided by GitHub - this is similar to viewing pages on GitHub itself but is cleaner on the edges.
- The build will add a homepage link to the top of each page. That is `h1`, so you first heading on the page should be an `h2`.
- There's an _Improve this page_ button in the bottom right of eac hpage.
- This pattern for a GH Pages site works using content in your `docs` directory. But you can also move everything to the root, such as if the entire repo is documentation, or if you are making a website that is not about documetnation. Just configure GH Pages to use the appropriate path.

## About

This project is built around using markdown content to make a website. 

This is great for non-developers to work on. No experience with Ruby, Jekyll, Liquid, HTML or CSS required. Those are all used internally, but no need to worry about that.

This repo is super light. No config needed. You don't need to setup a theme or a layout. GitHub will figure that out and will apply its standard theme to your GitHub Pages site. So will it will have a clean, white, mobile-friendly site with a heading.

The page you are currently viewing is `README.md`.

This project is a built around GitHub's functionality which lets you use GitHub Pages to render markdown (or HTML) files as a static website, from your root or `docs` folder.

Jekyll is still actually used to convert the files, but the project works with **no** typical Jekyll files such as layouts, themes, gems or configs. Github handles the CSS styling with a basic blue and white theme.

Note you can still use Jekyll Liquid templating. But the idea for this project is to avoid it and make a plain markdown docs site, which is easy for anyone to edit without Jekyll experience.

Your root page should be `index.md` or `README.md`. There is no navbar, so it is recommended to add a menu on your homepage which links to the other pages. You can always get back to the homepage using the link added for you at the top of every page.


### Convert to Jekyll

The approach here is also flexible - you can add a `_config.yml` file and a theme to turn your site in a proper Jekyll-based themed site.

You don't even have to add metadata to your pages - the layout will be set as `default.html`.


## Jekyll vs no Jekyll

### No Jekyll

If you want to upload plain HTML instead of `.md` files, create an empty `.nojekyll` file in your repo.

### Jekyll

If you want to upload markdown and have it rendered to HTML with Github's base styling, leave the `.nojekyll` file out so that Jekyll is used. Note that you don't need any config, Gemfile, theme etc. Just an `index.md` page and optionally more linked pages will work.

Jekyll will turn `index.md` into `index.html`. Any Liquid code for Jekyll can cause build errors, so since you're using Jekyll to parse you files you should use the `raw` tag to prevent the Liquid from being evaluated and rather render as plain text (typically in a codeblock).


## Credits

[![GitHub tag](https://img.shields.io/github/tag/MichaelCurrin/gh-pages-no-jekyll?include_prereleases=&sort=semver)](https://github.com/MichaelCurrin/gh-pages-no-jekyll/releases/)
[![License](https://img.shields.io/badge/License-MIT-blue)](#license)

Write Markdown or HTML pages and use GitHub's default theme for your site. No configuration needed. All you need is HTML, Markdown, and CSS knowledge - no need to use Jekyll templating or Liquid syntax.

## License

Released under [MIT](/LICENSE) by [@MichaelCurrin](https://github.com/MichaelCurrin).
