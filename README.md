<h1><img src="https://img.fortawesome.com/349cfdf6/logo-fa-pro.svg" alt="FontAwesome 6 Pro" width="50%"></h1>

# FontAwesome-6-PRO
###### Font Awesome Pro is commercial software that requires a paid license. (OR DOES IT!!!!)
###### Extract svgs.zip into same folder

### [OR]

##### Just Download The Pre-Packaged Files
#### Free
###### https://github.com/JeSTeRFLA/FontAwesome-6-PRO/raw/main/FontAwesome-6-FREE.7z

#### Pro
###### https://github.com/JeSTeRFLA/FontAwesome-6-PRO/raw/main/FontAwesome-6-PRO.7z

# Host Yourself - Web Fonts
### Set-Up with Web Fonts
###### The /webfonts folder contains all of the typeface files, i.e., the icons. 
###### The /css/all.css file contains the core styling plus all of the icon styles you'll need when using Font Awesome.
|   Which Files and Folders   |   What’s in there  |
|-----------------------------|--------------------|
|/fontawesome6/pro/webfonts   |   Icons as Web Fonts to be used with CSS   |
|/fontawesome6/pro/css   |   CSS files for using Web Fonts   |
|/fontawesome6/free/webfonts   |   Just the Free Icons as Web Fonts to be used with CSS   |
|/fontawesome6/free/css   |   CSS files for using just the Free Web Fonts   |

### Add Font Awesome Files to Your Project
###### Copy the /webfonts folder and the /css/all.css file into your project’s assets directory where other images and CSS are stored. 
###### You'll want to keep them in the same directory.

### Reference Font Awesome in Your Project
###### Add a link to the ./css/all.css file into the <head> of each template or page where you want to use Font Awesome.
```
<head>
  <!--load all Font Awesome styles -->
  <link href="./css/all.css" rel="stylesheet" />
</head>
```
### [OR]
  
### Using Only Certain Styles
|Icon Style | Web Font Filename | CSS Filename | Availability |
|-----------|-------------------|--------------|--------------|
|Font Awesome Brands  |  fa-brands-400.*  |  brands.css  |  Free |
|Font Awesome Solid  |  fa-solid-900.*  |  solid.css  |  Free |
|Font Awesome Regular  |  fa-regular-400.*  |  regular.css  |  Pro only |
|Font Awesome Light  |  fa-light-300.*  |  light.css  |  Pro only |
|Font Awesome Thin  |  fa-thin-100.*  |  thin.css  |  Pro only |
|Font Awesome Duotone  |  fa-duotone-900.*  |  duotone.css  |  Pro only |
  
###### Copy both the /webfonts and the /css folders into your project's static assets directory (or wherever you prefer to keep front-end assets or vendor stuff).
###### You can remove any styles' .css and web font files you don't plan on using if you'd like.

###### Add a reference to the core styling file (/css/fontawesome.css) and the CSS for individual styles (e.g., /css/brands.css) 
###### into the <head> of each template or page that you want to use Font Awesome on. 
###### Pay attention to the pathing of your project and where you moved the files in the previous step.
```
<head>
  <!-- Our project just needs Font Awesome Solid + Brands -->
  <link href="./css/fontawesome.css" rel="stylesheet" />
  <link href="./css/brands.css" rel="stylesheet" />
  <link href="./css/solid.css" rel="stylesheet" />
</head>
<body>
  <i class="fa-solid fa-user"></i>
  <!-- uses solid style -->
  <i class="fa-brands fa-github-square"></i>
  <!-- uses brand style -->
</body>
```

# Host Yourself - SVG + JS
### Set up with SVG+JS
###### The all.js file contains the core styling PLUS all of the icons in all the styles that you'll need when using Font Awesome. 
###### If you’re just using some styles, you can select just the JS files for the styles you need to cut down on file size and improve performance.
| Which Files and Folders  |  What’s in there |
|--------------------------|------------------|
| /fontawesome6/pro/js  |  Icons and scripts for each style, or all of them at once. |
| /fontawesome6/free/js  |  Just the Free icons and scripts for each style. |
  
### Add Font Awesome Files to Your Project
###### Copy all.js or individual style script files you want to use into your project’s static assets directory, 
###### or wherever you prefer to keep front-end assets or vendor stuff.
  
### Reference Font Awesome in Your Project
###### Link the files into the <head> of each template or page where you want to use Font Awesome icons.
```
<head>
  <!-- all.js loads all styles and icons -->
  <script defer src="./js/all.js"></script>
</head>
```
### [OR]
  
### Using Only Certain Styles
###### Want use only certain styles when using our SVG with JS framework? 
###### The /js folder contains the core styling and additional files for all of Font Awesome's style options- solid, regular, light, duotone, thin, and brands.
| Icon Style  |  JS Filename  |  Availability |
|-------------|---------------|---------------|
| Font Awesome Brands  |  brands.js  |  Free |
| Font Awesome Solid  |  solid.js  |  Free |
| Font Awesome Regular  |  regular.js  |  Pro only |
| Font Awesome Light  |  light.js  |  Pro only |
  
###### Copy the fontawesome.js loader and the .js files for the styles you'd like to use into your project's static assets directory 
###### (or where ever you prefer to keep front end assets or vendor stuff). We recommend referencing the fontawesome.js loader last.
```
<head>
  <!-- Our project just needs Font Awesome Solid + Brands -->
  <script defer src="./js/brands.js"></script>
  <script defer src="./js/solid.js"></script>
  <script defer src="./js/fontawesome.js"></script>
</head>
<body>
  <i class="fa-solid fa-user"></i>
  <!-- uses solid style -->
  <i class="fa-brands fa-github-square"></i>
  <!-- uses brand style -->
</body>

```
