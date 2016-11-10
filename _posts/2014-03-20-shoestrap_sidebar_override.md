---
layout: action
title:  "shoestrap_sidebar_override"
category: actions
permalink: actions/shoestrap_sidebar_override
---

The `shoestrap_sidebar_override` action can be used to replace the primary sidebar template.

### Example:
```php
<?php

function my_custom_sidebar() {
	// your custom sidebar template code
}
add_action( 'shoestrap_sidebar_override', 'my_custom_sidebar' );

?>
```

<hr>

* Location: [base.php](https://github.com/shoestrap/shoestrap/blob/master/base.php)