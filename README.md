The PHP SimpleCache Class is an easy way to cache 3rd party API calls. To use the class:

	require('simpleCache.php'); 
	$cache = new SimpleCache();
	$latest_tweet = $cache->get_data('tweet', 'http://search.twitter.com/search.atom?q=from:gilbitron&rpp=1');
	echo $latest_tweet;

Added ability to pass in cache time to get_data method. To be used as follows:

        $latest_tweet = $cache->get_data('tweet', 'http://search.twitter.com/search.atom?q=from:maxisnow&rpp=1', 600);
	

~~For more info see [this article](http://gilbertpellegrom.co.uk/post/592887883/php-simplecache-redux)~~ (no longer exists)
