Angular Image Fallback
======================

Angular directives that handles image loading, it has `fallback-src` to handle errors in image loading and `loading-src` for placeholder while the image is being loaded.

## Bower Download
`bower install angular-img-fallback`
  
## Installation
1. Download and import the plugin script.<br />
`<script src="lib/angular-img-fallback/angular.dcb-img-fallback.min.js"></script>`
2. Add `dcbImgFallback` to your angular app module dependencies list.<br />
`angular.module('myAngularApp', ['dcbImgFallback']);`
3. Add the `fallback-src` attribute to your img<br />
`<img ng-src="{{'path/to/img.jpg'}}" fallback-src />`


## Usage
Just add the `fallback-src` and the `loading-src` attributes to your `<img />` tags<br />
`<img ng-src="{{'path/to/img.jpg'}}" fallback-src loading-src />`<br />
Make sure you use `ng-src` as your image src attribute.


## Advanced options
- Simple usage, will replace to a default missing image placeholder<br />
`<img ng-src="{{'path/to/img.jpg'}}" fallback-src />`

- Custom fallback, will replace to your own custom missing image<br />
`<img ng-src="{{'path/to/img.jpg'}}" fallback-src="{{'path/to/fallback.jpg'}}" />`

- Loading placeholder, show a loading placeholder until image loads<br />
`<img ng-src="{{'path/to/img.jpg'}}" loading-src />`

- Custom Loading placeholder, show a custom image loading placeholder until image loads<br />
`<img ng-src="{{'path/to/img.jpg'}}" loading-src="{{'path/to/loading.jpg'}}" />`

- Or both! loading placeholder and a fallback source can work together<br />
`<img ng-src="{{'path/to/img.jpg'}}" loading-src fallback-src />`


## Icons license
Icons are provided from http://icomoon.io/ under the GNU General Public License v3.0<br />
http://www.gnu.org/licenses/gpl.html

## Contributing

To produce a distributable build, install Uglify JS by running `npm install uglify-js -g` and `uglifyjs angular.dcb-img-fallback.js -c -m -o angular.dcb-img-fallback.min.js`
