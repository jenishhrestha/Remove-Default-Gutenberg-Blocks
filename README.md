# Remove Default Gutenberg Blocks

> Comment the unnecessary block to remove it.

```
add_filter( 'allowed_block_types', 'gutenberg_blocks', 10, 2 );
function gutenberg_blocks( $allowed_blocks, $post ) {
 
	$allowed_blocks = array(
		'core/paragraph',
		'core/cover',
		'core/heading',
		'core/image',
		'core/gallery',
		'core/list',
		'core/quote',
		'core/audio',
		'core/file',
		'core/video',
		'core/pullquote',
		'core/code',
		'core/freeform', //classic editor
		'core/html', //Custom HTML
		'core/preformatted',
		'core/table',
		'core/verse',
		'core/columns',
		'core/button',
		'core/media-text',
		'core/more',
		'core/nextpage', //page break
		'core/separator',
		'core/spacer',
		'core/latest-posts',
		'core/shortcode',
		'core/archives',
		'core/categories',
		'core/latest-comments',
		'core/embed',
		'core-embed/hulu',
		'core-embed/twitter',
		'core-embed/youtube',
		'core-embed/facebook',
		'core-embed/instagram',
		'core-embed/wordpress',
		'core-embed/soundcloud',
		'core-embed/spotify',
		'core-embed/flickr',
		'core-embed/vimeo',
		'core-embed/animoto',
		'core-embed/cloudup',
		'core-embed/collegehumor',
		'core-embed/crowdsignal',
		'core-embed/dailymotion',
		'core-embed/funnyordie',
		'core-embed/imgur',
		'core-embed/issuu',
		'core-embed/kickstarter',
		'core-embed/meetup-com',
		'core-embed/mixcloud',
		'core-embed/photobucket',
		'core-embed/reddit',
		'core-embed/reverbnation',
		'core-embed/screencast',
		'core-embed/scribd',
		'core-embed/slideshare',
		'core-embed/smugmug',
		'core-embed/speaker-deck',
		'core-embed/ted',
		'core-embed/tumblr',
		'core-embed/videopress',
		'core-embed/wordpress-tv',
		'core-embed/ted',
	);
 
	return $allowed_blocks;
 
}
```