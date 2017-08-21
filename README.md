# Bootstrap Beta 4 Boilerplate
This is a collection of the public starter templates, using the [Bootstrap Beta 4](http://getbootstrap.com/) source files.

### Included Templates (so far):
- Starter-Template
- Jumbotron
- Navbar Examples
- Navbar Top
- Navbar Top Fixed
- Album
- Carousel
- Cover Page
 
For simplicity, the template related custom styles have been broken off onto there own matching individual css files. The'll need to be sorted out per individual project.

### Built In Workflow Tools
Assets include a dev/production workflow using Gulp.js, for compiling and reloading during development.

#### Included Dependencies:
| Dependency | More Info | Use |
| ------ | ------ | ------ |
| **gulp** | https://gulpjs.com/ | *workflow manager* |
| **gulp-util** | https://www.npmjs.com/package/gulp-util | *debugging* |
| **gulp-compass** | https://www.npmjs.com/package/gulp-compass | *compile sass* |
| **gulp-concat** | https://www.npmjs.com/package/gulp-concat | *concatenating sass and js files*  |
| **gulp-connect** | https://www.npmjs.com/package/gulp-connect | *live reload* |
| **browserify** | http://browserify.org/ | *compile js*|
| **gulp-if** | https://www.npmjs.com/package/gulp-if |*conditional statements*|
| **gulp-uglify** | https://www.npmjs.com/package/gulp-uglify |*minify css and js* |
| **gulp-minify-html** | https://www.npmjs.com/package/gulp-minify-html |*minify html* |
| **gulp-json-minify** | https://www.npmjs.com/package/gulp-json-minify |*minify json* |

### Instructions:
Clone repo and install dependencies.
```sh
$ npm install
```
### Tracking Changes with Git
Create remote repo and make any necessary updates to the `.gitignore` and `package.json` files.
```sh
$ git init
```
Set the remote repo as origin:
```sh
$ git remote add origin https://github.com/<USER-NAME>/<REPO-NAME>.git
```
Make first commit:
```sh
$ git commit -m "First commit." 
```
Push local changes to remote origin `-u` is only needed on first push to establish upstream:
```sh
$ git push -u origin master
```
### Development Environment
Start the Gulp process:
```sh
$ gulp
```
During development, Gulp will "watch" for changes in the `components/sass` and `components/scripts` directories. Any update will trigger a recompile and reload of the page.

### Project Completion
Upon project completion, change to a production environment from the terminal:
```sh
$ NODE_ENV=production gulp
```
... and Gulp will perform a final compile and minify of all included files for final packaging in the production directory.

---

### Update:
Trying to concat the popper.js with the bootstrap.js caused the dropdowns to malfunction. Removing it from the compile group and adding it solo. (may end up removing the whole js compile part of this for now)

Created using [Adam-P's Markdown Cheatsheet](https://github.com/adam-p/markdown-here/wiki/Markdown-Cheatsheet) and the [Dillinger](http://dillinger.io/) online readme preview tool.
(never did figure out how to insert a successful linebreak)