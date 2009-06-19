=== Simple Image Grabber ===
Contributors: c.bavota
Donate Link: https://www.paypal.com/cgi-bin/webscr?cmd=_s-xclick&hosted_button_id=1929921
Tags: posts, images from posts, retrieve images, get images, grab images, post images, pictures, photos
Requires at least: 2.7
Tested up to: 2.8
Stable tag: 1.0.1

== Description ==

Grabs an image from a post and displays it. Options include image width, height, class name and link. Can also display every image from a post if the $number variable is set to 'all'.

== Installation ==

1. Unzip the simple-image-grabber.zip file.
2. Upload the `simple-image-grabber` folder to the `/wp-content/plugins/` directory.
3. Activate the plugin through the 'Plugins' menu in WordPress.
4. Place `<?php images(); ?>` within the loop to grab your post's images.

== Frequently Asked Questions == 

1) How can I customize the Simple Image Grabber function?

The function from this plugin accepts five variables. 

The basic use of the function looks like: `<?php images('1'); ?>` or `<?php images(); ?>`

This will display the first image from your post, with its default width and height, no class name and a link to the post.

This is how the function looks with all variables:

`<?php images($number, $width, $height, $class, $link); ?>`

$number = the image you want to pull from your post, ie. the first image from the post ('1') or the second image from the post ('2') and so on. NOTE: If you use 'all', it will display all images from the post.

$width = the width of the displayed image

$height = the height of the displayed image

$class = the class name you would like to assign to the displayed image

$link = whether you would like the displayed image to link to the post or not

So, the following function:

`<?php images('2', '150', '200', 'alignleft', false); ?>`

would display the second image from a post (if there is one) with a width of 150px and a height of 200px, the class name alignleft and no link to the post.

The following:

`<?php images('all', '', '', 'alignright'); ?>`

would display all images from a post with their original width and height, a class name of alignright and a link to the post.

== Change Log ==

1.0.1 (2009-03-16)
<ul>
<li>Fixed issue with "All" variable</li>
</ul>

1.0 (2009-03-11)
Initial Public Release
