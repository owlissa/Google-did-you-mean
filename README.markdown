This Google did-you-mean script uses the mobil version of google to get suggested words. This might not be appreciated by google and it is the responsibility by the user to acquire any necessary permissions to use the script, provided as is.

## How to use native

1. Put the GoogleDidYouMean.php in your source folder and include the file in your project.
2. Instantiate new GoogleDidYouMean().
3. Call doSpellingSuggestion($phrase, $lang).

## How to use in wordpress

1. Put all files in your plugins directory.
2. Activate the plugin in wordpress.
3. Include following code anywhere you want to use google did you mean (example on the search result when no result was found).
		<?php if( function_exists('google_suggestion') ) { google_suggestion(); } ?>
	  
## Function interface

	function doSpellingSuggestion($phrase, $lang)

	$phrase - urlencoded phrase to lookup
	$lang - optional, supports "sv" for Swedish otherwise English