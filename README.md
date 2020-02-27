
# Parcel Github Pages Boilerplate

[![Publish Website](https://github.com/nicolas-van/parcel-github-pages-boilerplate/workflows/Publish%20Website/badge.svg)](https://github.com/nicolas-van/parcel-github-pages-boilerplate/actions?query=workflow%3A%22Publish+Website%22)

A Parcel boilerplate to automatically deploy on Github Pages using Github Actions.

[Demonstration website deployed here.](https://nicolas-van.github.io/parcel-github-pages-boilerplate/)

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
* Go in the settings of your repository and under `Github Pages` confirm that you want your Github Pages website to be built from the `gh-pages` branch. The settings page should then indicate you the URL of your deployed website, which should be `https://<your github account>.github.io/<the repository name>/` in most cases.
* Change something in your website to trigger a build and deployment (as example changing the text in `index.njk`).

Any following push to the `master` branch will automatically trigger the Github Actions workflow that will build and deploy your website to Github Pages.

### Commands

To install the requirements:

```
npm install
```

To start the project in development mode (automatically re-compiles the code):

```
npm start
```

To check the code with eslint (the CI will fail if this step doesn't pass):

```
npm run lint
```

To automatically fix the lint problems:

```
npm run lint:fix
```

## Contribution

[See the contribution guide.](./CONTRIBUTION.md)

## License

[See the license.](./LICENSE.md)

## Other Github Pages related projects

I'm a fan of Github Pages for the possibilities it offers to anyone to publish a website for free. I have multiple projects that could be of interest if that's your case too:

* [Easy Markdown to Github Pages](https://nicolas-van.github.io/easy-markdown-to-github-pages/)
* [Bootstrap 4 Github Pages](https://nicolas-van.github.io/bootstrap-4-github-pages/)
