# Brand Styleguide

Welcome to the Brand Styleguide!

##How to use CSS Styles

Our Styleguide allows you to easily select standardized CSS classes you would like to include and easily inject them into your project. Styles are built in [SCSS] (http://sass-lang.com/) and may be found in the folder `public/css/`. Once you have SCSS installed, you'll be able to cherry pick from our pre-built SCSS files and generate your own CSS files.

#### Setup SCSS

Download SCSS from [here] (http://sass-lang.com/install). If you have Ruby, running `sudo gem install sass` should do the trick, else first install [Ruby] (https://www.ruby-lang.org/en/documentation/installation/).

Go into the folder `public/css/`. Here you'll find many SCSS files. Browse through the classes, and when you're ready to start your own, create a file inside this folder called `localstyle.scss`. Now enter these imports at the beginning of the file:

```
@import './_boilerplate.scss';
```

This import line will include all the variable dependencies as well as resets, typography, and general boilerplate classes. Now, if you would like to include other files, simply add another line of `@import /path/of/file` to add that SCSS file. However, if you'd like to cherry pick, from here on out, you can copy paste specific classes from the pre-built SCSS classes or write your own.

Importantly, you're now able to use the variables defined in `_variables.scss`. To use a variable: `$variable-name`.

After you're satisfied with your classes, you're ready to convert to CSS! Go to the css folder in your Terminal. Now run:

```
sass localstyle.scss localstyle.css
```

Now you have a `localstyle.css` file! Drag this file into your project, include it as a link in your HTML and you're all set!

##How to use JS Files

