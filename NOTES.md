# NetNinja's "Bootstrap 5" Notes

## New Features in Bootstrap 5:

- Has dropped jQuery (and uses vanilla JS for its components)
- Forms have been revamped and given more specific support (especially in the documentation)
- Right-To-Left (RTL) support has been added (for human languages that read RTL)
- New utility classes (for positioning, font size, border radius, etc.)
- Minor changes to some components & grid (Note: Jumotron is gone, but you can still replicate it with other classes)
- Bootstrap icons (instead of FontAwesome etc)
- Two new components - Offcanvas (a "slide-in sidebar"... which can also come in from top and bottom) and Accordian (where an unordered list can be clicked to show/hide further drop-down info)
- Extra color variables

## [Getting Started](https://getbootstrap.com/docs/5.2/getting-started/introduction/): adding _Bootstrap_ to your project

If you want to import using their CDN ...

1. Add the following to your Index.html's `<style>` section (in `<head>`):

< link href="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/css/bootstrap.min.css" rel="stylesheet" integrity="sha384-Zenh87qX5JnK2Jl0vWa8Ck2rdkQ2Bzep5IDxbcnCeuOxjzrPF/et3URy9Bv1WTRi" crossorigin="anonymous">

> Note: make sure your `<head>` section has a meta tag with `name="viewport"`, like `<meta name="viewport" content="width=device-width, initial-scale=1">`

2. Add the following to your Index.html/webpage's `<body>`:

`<script src="https://cdn.jsdelivr.net/npm/bootstrap@5.2.2/dist/js/bootstrap.bundle.min.js" integrity="sha384-OERcA2EqjJCMA+/3y+gxIOqMEjwtxJY7qPCqsdltbNJuaOe923+mo//f6V8Qbsw3" crossorigin="anonymous"></script>`

If you want to install as a package:

1. Run `npm install bootstrap` / `yarn add bootstrap`
2. Add `import "bootstrap/dist/css/bootstrap.min.css";` and `import "bootstrap/dist/js/bootstrap.js";`
   - to your 'main.js' (in Vue)

## [Getting Started](https://icons.getbootstrap.com/#install): adding Bootstrap _Icons_ to your project

If you want to import using their CDN ...

1. Add the following to your Index.html's `<style>` section (in `<head>`):

   < link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css">

2. Add the following to your styles.css:

   @import url("https://cdn.jsdelivr.net/npm/bootstrap-icons@1.9.1/font/bootstrap-icons.css");

If you want to install as a package:

1. Run `npm i bootstrap-icons` / `yarn add bootstrap-icons`,
2. Add `import "bootstrap-icons/font/bootstrap-icons.css";` to your 'main.js'

## Getting Started: What to know ...

## Error Fixes:

- In general, be sure that you are importing the same version of Bootstrap at all points (instead of mix-matching Bootstrap 4 with, say, Bootstrap 5, etc.)

## Bootstrap Syntax (General):

Re: your browser's vanilla stylings for HTML tags:

- Bootstrap, when first installed, will clear-out the browser's initial stylings using a ["Reboot"](https://getbootstrap.com/docs/5.2/content/reboot/). This means that not only do you have the classes of Bootstrap made available to you (say, `class="h3"`) - you also have new vanilla styling injected-in ... so in theory, you could set an < h2> to look like an h3:
  `<h2 class="h3">This h2 tag is made to look like an h3 tag, using a *class* to override Bootstrap's vanilla styling - which is overriding HTML's vanilla styling 😵 </h3>`

For specific syntax:

- Check the demos in this app & Bootstrap's documentation for specific syntax & component structuring

<!-- ##### TEMPLATE for further notes:

## REPLACE (Vid #1, 00:00)

What is it?

-

How do you do it?

- f
  > - Check project_1,

Example: -->
