#GULP
https://css-tricks.com/gulp-for-beginners/

```
$ npm install gulp-sass --save-dev
$ sudo npm install gulp -g
```

```
// Include gulp
var gulp = require('gulp');
var sass = require('gulp-sass');

// Default Task
gulp.task('default', ['sass']);

gulp.task('watch', function(){
  gulp.watch('sass/partials/*.sass', ['sass']); 
})

gulp.task('sass', function(){
  return gulp.src('sass/app.sass')
    .pipe(sass()) // Using gulp-sass
    .pipe(gulp.dest('css/'))
});
```
