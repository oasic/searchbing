![Puffin](http://photos-g.ak.fbcdn.net/hphotos-ak-snc1/hs166.snc1/6216_704615592619_7804626_41719230_39698_n.jpg)


A Ruby interface to the Bing Search API.

find the [gem](https://rubygems.org/gems/searchbing) on rubygems.org



## Installation
    gem install searchbing


Configuration
=============
You can create a new account for the Bing Search API and obtain account key [here](http://www.bing.com/developers/)

Usage
============
1. create a new search object from the Bing class. Enter your recently obtained account key, the number of results you would like, and the search type.
2. valid search types include: Image, Web, or Video. The first letter must be capitalized
3. the searchbing gem relies on the open-uri, net/http, and json gems.

Example: Interactive Ruby Shell
===============
## Require the gem in your shell session
   	require 'searchbing'
## Create a new search object.
	animals = Bing.new('your_account_key_goes_here', 10, 'Image')
## Retrieve the results for a given term.
	bing_results = animals.search("lion")
## parse the results 
	puts bing_results[0]["Thumbnail"]["MediaUrl"] # puts url of thumbnail  


	  

  




