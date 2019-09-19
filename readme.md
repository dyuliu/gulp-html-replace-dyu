I make a slight change on the original plugin "https://github.com/VFK/gulp-html-replace.git".

- remove the two unnecessary blank lines used for padding. 



#### Example

------

index.html

```html
<!DOCTYPE html>
<html>
    <head>
    <!-- build:css -->
        content will be added here
    <!-- endbuild -->
    </head>
```



The outputs of the original plugin:

```html
<!DOCTYPE html>
<html>
    <head>
    A blank line will be added here
    <!-- build:css -->
    <link rel="stylesheet" href="css/normalize.css">
    <link rel="stylesheet" href="css/main.css">
    <!-- endbuild -->
 	A blank line will be added here
    </head>
```



The outputs of the current version:

```html
<!DOCTYPE html>
<html>
    <head>
    <!-- build:css -->
    <link rel="stylesheet" href="css/normalize.css">
    <link rel="stylesheet" href="css/main.css">
    <!-- endbuild -->
    </head>
```

