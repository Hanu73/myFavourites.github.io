Angular Material

Installing Build (Distribution Files)

Bower

For developers not interested in building the Angular Material library... use bower to install and use the Angular Material distribution files.

Change to your project's root directory.

To get the latest stable version, use Bower from the command line.

bower install angular-material

To get the most recent, latest committed-to-master version use:

bower install angular-material#master Visit Bower-Material for more details on how to install and use the Angular Material distribution files within your own local project.

CDN

CDN versions of Angular Material are now available at Google Hosted Libraries.

With the Google CDN, you will not need to download local copies of the distribution files. Instead simply reference the CDN urls to easily use those remote library files. This is especially useful when using online tools such as CodePen, Plunkr, or JSFiddle.

<!-- Angular Material CSS now available via Google CDN; version 1.0.7 used here -->
<link rel="stylesheet" href="https://ajax.googleapis.com/ajax/libs/angular_material/0.11.2/angular-material.min.css">
<!-- Angular Material Dependencies -->
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular.min.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular-animate.min.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular-aria.min.js"></script>


<!-- Angular Material Javascript now available via Google CDN; version 1.0.7 used here -->
<script src="https://ajax.googleapis.com/ajax/libs/angular_material/1.0.7/angular-material.min.js"></script>
Developers seeking the latest, most-current build versions can use GitCDN.link to pull directly from the distribution GitHub Bower-Material repository:

<!-- Angular Material CSS using GitCDN to load directly from `bower-material/master` -->
<link rel="stylesheet" href="https://gitcdn.link/repo/angular/bower-material/master/angular-material.css">
<!-- Angular Material Dependencies -->
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular-animate.js"></script>
<script src="https://ajax.googleapis.com/ajax/libs/angularjs/1.3.15/angular-aria.js"></script>

<!-- Angular Material Javascript using GitCDN to load directly from `bower-material/master` -->
<script src="https://gitcdn.link/repo/angular/bower-material/master/angular-material.js"></script>
Once you have all the necessary assets installed, add ngMaterial as a dependency for your app:

angular.module('myApp', ['ngMaterial']);
