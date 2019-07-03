# php-cli-iterm-image-renderer
Render images with PHP in your iterm2 console

## usage

```
#!/usr/bin/env php
<?php

use Technodelight\ITermImage\Image;
$image = Image::fromUri('https://picsum.photos/200', 200);
if (!empty($image)) {
    echo $image;
}
```
Running the above script will render a random picsum image in your terminal, 200 px wide.

## requirements

This library was built to work with the famous iTerm2 OS X application.
It has a basic fallback version to render the URI instead of the image, if the current
iTerm does not support displaying images (or you're not using iTerm2 at all).