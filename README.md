yii2-context-menu
=================

A context menu extension for Yii framework 2.0 that allows you to add and render a context menu to any element on the page. A context menu 
is a pop up menu that one initiates on any element by right clicking the mouse in that target element. This widget is a wrapper for the 
[bootstrap-contextmenu plugin](https://github.com/sydcanem/bootstrap-contextmenu) which is styled for Bootstrap 3. The widget uses 
the `\yii\bootstrap\Dropdown` widget to generate a dropdown menu.

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