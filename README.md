Angular Image Fallback
======================

Angular directives that handles image loading, it has `image-holder` to handle errors in image loading and `image-loading` for placeholder while the image is being loaded.
  
## Installation
1. Download and import the plugin script.<br />
`<script src="lib/angular-img-fallback/angular.dcb-img-fallback.min.js"></script>`
2. Add `dcbImgFallback` to your angular app module dependencies list.<br />
`angular.module('myAngularApp', ['dcbImgFallback']);`
3. Add the `fallback-src` attribute to your img<br />
`<img image="{{'path/to/img.jpg'}}"  />`


## Usage
Just add the `image` attribute to your `<img />` tags<br />
`<img image="{{'path/to/img.jpg'}}"  />`<br />
Make sure you use `ng-src` as your image src attribute.


## Advanced options


 - default:<br />
`<img image="{{image.url}}" />`

 - with custom loading placeholder:<br />
`<img image="{{image.url}}" image-loading="/image/loading.gif" />`

 - with custom fallback placeholder:<br />
`<img image="{{image.url}}" image-holder="/image/error.png" />`

 - with custom fallback and loading placeholders:<br />
`<img image="{{image.url}}" image-loading="/image/loading.gif" image-holder="/image/error.png" />`



## Icons license
Icons are provided from http://icomoon.io/ under the GNU General Public License v3.0<br />
http://www.gnu.org/licenses/gpl.html
