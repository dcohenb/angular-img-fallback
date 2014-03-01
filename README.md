Angular Image Fallback
======================

Utility to work with loading images, has `fallback-src` to handle erros in image loading and `loading-src` for images loading placeholders.


## Installation
1. Download and import the plugin script.<br />
`<script src="lib/angular-img-fallback/angular.dcb-img-fallback.min.js"></script>`
2. Add `dcbImgFallback` to your angular app module dependencies list.<br />
`angular.module('myAngularApp', ['dcbImgFallback']);`
3. Add the `fallback-src` attribute to yout img<br />
`<img ng-src="path/to/img.jpg" fallback-src />`


## Usage
Just add the `fallback-src` and the `loading-src` attributes to your `<img />` tags<br />
`<img ng-src="path/to/img.jpg" fallback-src loading-src />`<br />
Make sure you use `ng-src` as your image src attribute.


## Advanced options
- Simple usage, will replace to a default missing image placeholder<br />
`<img ng-src="path/to/img.jpg" fallback-src />`

- Custom fallback, will replace to your own custom missing image<br />
`<img ng-src="path/to/img.jpg" fallback-src="path/to/fallback.jpg" />`

- Loading placeholder, show a loading placeholder until image loads<br />
`<img ng-src="path/to/img.jpg" loading-src="path/to/fallback.jpg" />`

- Custom Loading placeholder, show a custom image loading placeholder until image loads<br />
`<img ng-src="path/to/img.jpg" loading-src="path/to/loading.jpg" />`


## Icons license
Icons are provided from http://icomoon.io/ under the GNU General Public License v3.0<br />
http://www.gnu.org/licenses/gpl.html
