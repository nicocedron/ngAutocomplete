# ngAutocomplete
AngularJS Autocomplete

Live Example: [demo](http://demo.jankuri.com/ngAutocomplete)

#### Installation
    $ bower install ngAutocomplete-jkuri
    
#### Configuration

```html
<!DOCTYPE html>
<html ng-app="app">
<head>
  <link rel="stylesheet" type="text/css" href="bower_components/ngAutocomplete-jkuri/src/css/ngAutocomplete.css">
</head>
<body ng-controller="Ctrl as ctrl">

<ng-autocomplete ng-model="ctrl.keyword"
	   url="data/example_data.json"
	   search-property="title"
	   max-results="10"
	   delay="300"
	   min-length="2"
	   allow-only-results="true"
	   theme="red"
	   placeholder="Išči ...">
</ng-autocomplete>

<script type="text/javascript" src="https://ajax.googleapis.com/ajax/libs/angularjs/1.4.0/angular.min.js"></script>
<script type="text/javascript" src="bower_components/ngAutocomplete-jkuri/src/js/ngAutocomplete.min.js"></script>
<script type="text/javascript">
var app = angular.module('app', ['jkuri.autocomplete']);
app.controller('Ctrl', [function() {
	var self = this;
}]);
</script>
</body>
</html>
``` 

For more information and example please see: [demo](http://demo.jankuri.com/ngAutocomplete)
