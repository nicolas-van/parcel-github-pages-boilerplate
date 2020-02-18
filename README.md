
# Parcel Github Pages Boilerplate

[![Publish Website](https://github.com/nicolas-van/parcel-github-pages-boilerplate/workflows/Publish%20Website/badge.svg)](https://github.com/nicolas-van/parcel-github-pages-boilerplate/actions?query=workflow%3A%22Publish+Website%22)

[Demonstration website deployed here.](https://nicolas-van.github.io/parcel-github-pages-boilerplate/)

A Parcel boilerplate to automatically deploy on Github Pages using Github Actions.

## Included tools and libraries

* [Parcel](https://parceljs.org/): The zero configuration web application bundler
* [Babel](https://babeljs.io/): The Javascript compiler. It's used implicitly by Parcel. Already contains a configuration for [React](https://reactjs.org/).
* [Sass](https://sass-lang.com/): The CSS pre-compiler.
* [Bootstrap 4](https://getbootstrap.com/): The CSS framework, its SCSS files are compiled by Parcel which allows to override the theme. (The provided theme is [Cerulean from Bootswatch](https://bootswatch.com/cerulean/).)
* [Eslint](https://eslint.org/) with the [standard](https://standardjs.com/) configuration: Because everyone should use a linter nowadays.
* [Nunjucks](https://mozilla.github.io/nunjucks/): The best Javascript template engine available. Useful to have multiple different pages on your website.
* [Font Awesome](https://fontawesome.com/): Everyone needs icons right ? The provided version does not use a CDN, they are automatically bundled during the build.

## How to use it

* Fork this repository and publish it in a new Github repository.
* Go in the settings of your repository and under `Github Pages`, confirm that you want your Github Pages website to be built from the `gh-pages` branch.
* Change something in your website to trigger a build and deployment (as example changing the text in `index.njk`).

By following these steps the settings page should indicate you the URL of your deployed website, which should be `https://<your github account>.github.io/<the repository name>/`.
