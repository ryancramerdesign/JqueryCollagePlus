# CollagePlus for ProcessWire

[CollagePlus](http://ed-lea.github.io/jquery-collagePlus/) is a jQuery plugin by Ed Lea. 
It takes a list of images and converts it to a nicely formatted grid. 

With this module, we use the CollagePlus plugin to produce nice grid output for 
ProcessWire image selection. This applies to the images that you select when 
clicking the image icon from the rich text editor (TinyMCE or CKEditor). 

To use, simply install the module and it is ready to go. 

## Other uses

This module can also serve as a wrapper to the jQuery CollagePlus 
library for your own needs. To use it that way you would just:

```
$collagePlus = $modules->get('JqueryCollagePlus'); 
$collagePlus->load(); 
```
That load() function above populates `$config->scripts` and
`$config->styles` with all the needed javascript/styles.
Of course, you could also just reference those files yourself,
if preferred, example: 

```
<script src='<?=$config->urls->JqueryCollagePlus?>collagePlus-0.3.0/jquery.collagePlus.js'></script>
```

## Credits

[CollagePlus jQuery plugin](http://ed-lea.github.io/jquery-collagePlus/)
is by [Ed Lea](http://qiip.me/edlea/).

The idea for this usage (in the admin image selection) is by
[adamspruijt](http://modules.processwire.com/authors/adamspruijt/),
as he made use of it in his Unify admin theme. I wanted to use the 
same output in other admin themes, so this module was the result.

The ProcessWire module is by Ryan Cramer.

