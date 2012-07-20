Install
-------

To install **lyiightbox** you could copy his files in folder

    /protected/extensions/lyiightbox

lyiightbox.LightBox2
--------------------

To use this widget you can call it setting some parametes. If you want, you can 
also hide some images with "visible" option. By default visible is set on true. 
And if you want, you can group images with 'group' value. By default this value 
is 'default'

    <?php
            $this->widget('ext.lyiightbox.LyiightBox2', array(
                'thumbnail' => '/path/to/thumb/images.jpg',
                'image' => '/path/to/image/image.jpg',
                'title' => 'Sample Image 1.',
		'visible' => true,
		'group' => 'myOwnGallery'
            ));
    ?>

lyiightbox.Galleryii
--------------------

Since version 1.1 where added a new feature: gallery. By default, you have to 
put your images in /images/galleryii/ folder. Thumbnail will be placed in 
/images/galleryii/thumbnails folder. Big images where be placed in 
/images/galleryii/images folder. Thumb, and image, must have the same filename.

    <?php
	$this->widget('ext.lyiightbox.Galleryii');
    ?>

If you want, you can configure this new feature. Maybe you need to place your 
gallery in a different place!

    <?php
	$this->widget('ext.lyiightbox.Galleryii', array(
            'rootFolder' => '/place/of/gallery', // by default '';
            'baseFolder' => '/images/galleryii', // by default '/images/galleryii';
            'thumbnails' => '/thumbnails',	     // by default '/thumbnails';
            'images' => '/images'		     // by default '/images';
	));
    ?>