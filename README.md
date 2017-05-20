## Project gulp starter - Arkadiusz Chatys [www.iamarek.com](http://www.iamarek.com)
##### Gulp starter based on starter by Una Kravets (https://github.com/una)

## What's included:

- Scss support (gulp-sass)
- Minify CSS (gulp-minify-css)
- Minify JavaScript (gulp-uglify)
- Minify HTML (gulp-minify-html)
- Minify images (gulp-imagemin)
- Linting of JavaScript (gulp-jshint)
- Scss support (gulp-sass-lint)
- Cache (gulp-cached)
- Autoprefixer (gulp-autoprefixer)
- Browser Sync (browser-sync)
- Log size of project (gulp-size)
- GitHub pages deploy (gulp-gh-pages)
- Injecting Partials (gulp-inject-partials)
- Concatenating CSS/JavaScript files (gulp-useref)

## How to start:

1. Clone this repository running `git clone git@github.com:iamarek/project-gulp-starter.git` in your terminal.
2. Go to folder inside running `cd project-gulp-starter`.
3. Run `npm install` to install all dependencies
4. Run `gulp` to start working on project

## Commands

- `gulp` - to run dev environment with localhost:3000
- `gulp prod` - to minify JavaScript
- `npm test` - to run Mocha tests

## Concatenating files

To concatenate JavaScript files go to your html file and add all files in order inside of tags like so:

```
<!-- build:js js/main.js -->
  <script src="js/jquery.js"></script>
  <script src="js/main.js"></script>
<!-- endbuild -->
```

To concatenate CSS files go to your html file and add all files in order inside of tags like so:

```
<!-- build:css css/main.css -->
  <link rel="stylesheet" href="css/font-awesome.css">
  <link rel="stylesheet" href="css/main.css">  
<!-- endbuild -->
```

## Including Partials

To include partial create keyword `{% include path/to/your/file.html %}`.

## Mocha testing

To use Mocha tests run `npm test` in your terminal
