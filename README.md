yii2-context-menu
=================

A context menu extension for Yii framework 2.0 that allows you to add and render a context menu to any element on the page. A context menu 
is a pop up menu that one initiates on any element by right clicking the mouse in that target element. This widget is a wrapper for the 
[bootstrap-contextmenu plugin](https://github.com/sydcanem/bootstrap-contextmenu) which is styled for Bootstrap 3. The widget uses 
the `\yii\bootstrap\Dropdown` widget to generate a dropdown menu.

> NOTE: This extension depends on the [kartik-v/yii2-widgets](https://github.com/kartik-v/yii2-widgets) extension which in turn depends on the
[yiisoft/yii2-bootstrap](https://github.com/yiisoft/yii2/tree/master/extensions/bootstrap) extension. Check the 
[composer.json](https://github.com/kartik-v/yii2-context-menu/blob/master/composer.json) for this extension's requirements and dependencies. 
Note: Yii 2 framework is still in active development, and until a fully stable Yii2 release, your core yii2-bootstrap packages (and its dependencies) 
may be updated when you install or update this extension. You may need to lock your composer package versions for your specific app, and test 
for extension break if you do not wish to auto update dependencies.

### Demo
You can see detailed [documentation](http://demos.krajee.com/context-menu) on usage of the extension.

## Installation

The preferred way to install this extension is through [composer](http://getcomposer.org/download/).

Either run

```
$ php composer.phar require kartik-v/yii2-context-menu "dev-master"
```

or add

```
"kartik-v/yii2-context-menu": "dev-master"
```

to the ```require``` section of your `composer.json` file.

## Usage

### ContextMenu

```php
use kartik\cmenu\ContextMenu;
ContextMenu::begin([
    'items' => [
        ['label' => 'Action', 'url' => '#'],
        ['label' => 'Another action', 'url' => '#'],
        ['label' => 'Something else here', 'url' => '#'],
        '<li class="divider"></li>',
        ['label' => 'Separated link', 'url' => '#'],
    ],
]); 
// fill in any content within your target container
ContextMenu::end();
```

## License

**yii2-context-menu** is released under the BSD 3-Clause License. See the bundled `LICENSE.md` for details.