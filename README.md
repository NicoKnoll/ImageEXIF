ImageEXIF
=========

Adds the EXIF data of an image to it's object.

There are some aliases (e.g. "exposureTime" and "tv") and unformatted values (e.g. "focalLengthUnformatted") included.

_Example for which EXIF data get's added:_
```json
{
"aperture":5.6,
"apertureUnformatted":"56\/10",
"av":5.6,
"exposure":"1\/320",
"exposureTime":"1\/320",
"tv":"1\/320",
"shutterTime":"1\/320",
"cameraMake":"Canon",
"cameraModel":"Canon EOS 1100D",
"name":"image",
"filename":"image.jpg",
"filesize":2346963,
"mimeType":"image\/jpeg",
"height":2056,
"width":3088,
"artist":null,
"photographer":null,
"comment":"",
"copyright":null,
"flash":"Flash did not fire, compulsory flash mode",
"flashUnformatted":16,
"focalLength":"250mm",
"focalLengthUnformatted":250,
"iso":640,
"ISO":640,
"orientation":1,
"orientationUnformatted":1,
"date":"2013-10-27",
"time":" 15:53:07",
"timestamp":1382885587,
"whiteBalance":"Daylight",
"whiteBalanceUnformatted":1
}
```

_How to use (example):_

```php
<?php
$image = $page->images->first();
echo 'ISO: '.$image->EXIF->iso; // $image->exif->iso would work, too
?>
```

