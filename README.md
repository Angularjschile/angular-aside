angular-aside
=============

Off canvas side menu to use with ui-bootstrap. Extends ui-bootstrap's $modal provider.

###[Live Demo](http://plnkr.co/edit/w8Clzab6jJf6fPMHEXpP?p=preview)

##Install

- Install with bower:
```bash
 $ bower install angular-aside
```
- Include css/js in html.


##Usage

```js
 angular.modoule('myApp', ['ui.bootstrap', 'ngAside']);
```

```js
angular.module('myApp')
  .controller('MyController', function($scope, $aside) {
    var asideInstance = $aside.open({
      templateUrl: 'aside.html',
      controller: 'AsideCtrl',
      placement: 'left',
      size: 'lg'
    });
  });
```

Supports all configuration that `$modal` has. Can be used with both `template` and `templateUrl`.


##Additional Config
- `placement` - Aside placement can be `left` or `right`.


##Credits
- [Angular UI Bootstrap](angular-ui.github.io/bootstrap/)
- [Animate.css](http://daneden.github.io/animate.css/)


##Author

İsmail Demirbilek ([@dbtek](https://twitter.com/dbtek))
