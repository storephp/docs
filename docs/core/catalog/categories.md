---
title: Categories
sidebar_position: 1
---

# Categories

You can install StorePHP Core via composer

## The Namespace

```php
<?php

use Store\Models\Product\Category;
```

## Methods

### Create new category

```php
<?php

use Store\Models\Product\Category;

$category = Category::create([
    'parent_id' => $validatedData['parent_id'], // null
    'slug' => 'slug', // slug
]);

$category->name = $validatedData['name'];

$category->save();
```
