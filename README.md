# jarvis-ss-alternative
This is a fix for smooth scroll issue on Chrome 61, for Jarvis Wordpress Theme

Just put the scroller.js file inside ../themes/jarvs-wp/js/ folder <b>NOT in the child theme folder</b>

Comment the call for smoothscroll.js in the functions.php:101 file.

Register the new script in functions.php:102 file adding:
wp_register_script('rnrSmoothScroll', RNR_INDEX_JS .'/scroller.js', true);

That's it all!
