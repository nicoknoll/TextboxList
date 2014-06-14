TextboxList
===========

**This inputfield adds Facebook like TextboxLists to ProcessWire.**

![](https://processwire.com/talk/uploads/monthly_01_2012/post-5023-132614281893.png)

The field's contents are stored as a comma separated list in the database. 

Here is a small example on how to output it in your template:

```php
// "tags" is the name of the field
$tags = $page->tags;

// split the comma seperated list
foreach(explode(',', $tags) as $tag) {
  echo trim($tag).'<br>';
}

```
