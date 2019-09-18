# Genesis Starter Theme (Sass & Gulp)
The Genesis Sample theme, Sassified, with a Gulp-driven workflow. 

### Installation
1. Clone or download the repository
2. Run npx wpgulp (to install WP Gulp (thanks to https://github.com/ahmadawais/WPGulp for putting this nice package together))
3. Configure the project paths and other variables inside the wpgulp.config.js file. This is a compulsory step. (See below for specific paths for this theme)
4. Run npm install to install dependencies
5. Run npm start to begin gulp process


### Specifics
**wpgulp.config.js paths**

```
.........

	// Project options.
	projectURL: 'localhost:8888', // Local project URL of your already running WordPress site. Could be something like wpgulp.local or localhost:3000 depending upon your local WordPress setup.
	productURL: './', // Theme/Plugin URL. Leave it like it is, since our gulpfile.js lives in the root folder.
	browserAutoOpen: false,
	injectChanges: true,

	// Style options.
	styleSRC: './assets/sass/style.scss', // Path to main .scss file.
	styleDestination: './assets/css', // Path to place the compiled CSS file. Default set to root folder.
	outputStyle: 'compact', // Available options → 'compact' or 'compressed' or 'nested' or 'expanded'
	errLogToConsole: true,
	precision: 10,

	// JS Vendor options.
	jsVendorSRC: './assets/js/vendor/*.js', // Path to JS vendor folder.
	jsVendorDestination: './assets/js/', // Path to place the compiled JS vendors file.
	jsVendorFile: 'vendor', // Compiled JS vendors file name. Default set to vendors i.e. vendors.js.

	// JS Custom options.
	jsCustomSRC: './assets/js/custom/*.js', // Path to JS custom scripts folder.
	jsCustomDestination: './assets/js/', // Path to place the compiled JS custom scripts file.
	jsCustomFile: 'custom', // Compiled JS custom file name. Default set to custom i.e. custom.js.

	// Images options.
	imgSRC: './assets/images/raw/**/*', // Source folder of images which should be optimized and watched. You can also specify types e.g. raw/**.{png,jpg,gif} in the glob.
	imgDST: './assets/images/', // Destination folder of optimized images. Must be different from the imagesSRC folder.

	// Watch files paths.
	watchStyles: './assets/sass/**/*.scss', // Path to all *.scss files inside css folder and inside them.
	watchJsVendor: './assets/js/vendor/*.js', // Path to all vendor JS files.
	watchJsCustom: './assets/js/custom/*.js', // Path to all custom JS files.
	watchPhp: './**/*.php', // Path to all PHP files.
  
  ........
  ```
  
