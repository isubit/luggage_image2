This module is intended to update luggage sites to use the CKEditor Image2
plugin to support image captions.

Warnings:

* This will remove the feature where users are able to adjust image hSpace and
vSpace options.

* Users will once again be able to modify the URL of the image and possibly
link to external resources. We highly discourage displaying images from servers
we don't have control over.

* We would like to change default luggage to use Image2 in the future as well.
An upgrade path from this to whatever future solution will not be developed.

* We're sure there are unknown bugs.

Use at your own risk.

Installation:

* Enable luggage_image2

* Enable image2 CKEditor plugin at admin/config/content/ckeditor/edit/WYSIWYG

* Go to the WYSIWYG Filter Text format at admin/config/content/formats/wysiwyg

* Add the following to the WYSIWYG Filter HTML elements and attributes:

,
figure[class|style],figcaption


* Add the following to the Rules fo Class names

image,
rtecenter,
rteright

* Apply appropriate CSS styles as you see fit in a site-specific module or
wherever you like to place CSS.
