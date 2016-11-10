---
layout: filter
title:  "shoestrap_widgets_class"
category: filters
permalink: filters/shoestrap_widgets_class
---

You can use the `shoestrap_widgets_class` filter to change the class of the widgets, or add your own classes to them.

### Examples:

If you want to **replace** the default class of the widgets, you can use the following code:

```php
<?php

function custom_replace_widget_class() {
	return 'my-class';
}
add_filter( 'shoestrap_widgets_class', 'custom_replace_widget_class' );
?>
```

If on the other hand you want to **add** a class to the widgets, you can use something like this:

```php
<?php

function custom_add_widget_class( $class ) {
	return $class . ' my-class';
}
add_filter( 'shoestrap_widgets_class', 'custom_replace_widget_class' );
?>
```

<hr>
* Location: [lib/widgets.php](https://github.com/shoestrap/shoestrap-3/blob/development/lib/widgets.php)
* Related: [shoestrap\_widgets\_before\_title](/filters/shoestrap_widgets_before_title), [shoestrap\_widgets\_after\_title](/filters/shoestrap_widgets_after_title)