# Intro
This repo is used to record some search skills for googling.


# advanced search skills

The skills to be introduced may be roughly divided into three categories: location-directed, content-directed and others.

- ## location-directed 
In this way, we can filter pages according the location. specifically, we can use the site and url of a page
to control the location.

- ### site
By its very name, we can tune our search to make result limited to some specific location and by location, 
I mean the domain of web pages. In google, we can use **site** keyword to achieve this goal.

For example, we wanna search pages which contain **javascript prototype**, we can type search like this:

![before_use_site_keyword](./pictures/before_use_site_keyword.png)

As we can see in the picture above, the result pages do contain **javasript and/or prototype**, but 
we now want pages only from some domain, say ***stackoverflow.com***, for pages from this domain are more likely
have high-quality contents we may need, so we can tune our search like this:

![after_use_site_keyword](./pictures/after_use_site_keyword.png)

So the result pages now are all from the same domain of ***stackoverflow.com***.

- ### url
We can further do something on the url of pages. And in google we have two related operator: inurl and allinurl.

- #### inurl

For example, we wanna the url of pages containing **zju and/or cs** , so we can construct our search like this:

![inurl_example](./pictures/inurl_example.png)

- #### allinurl
The key difference between inurl and allinurl is that the latter one requires all the keywords be contained in url, while
the former require at least one of keywords represent in url. The following picture shows the result with using **allinurl**:

![allinurl_example](./pictures/allinurl_example.png)

As far as I know, we can tune the site and url of pages to make result pages more closer to what we expected as to the 
location of pages.

- ## content-directed 
In this way, we can tune our search according the title, body, filetype of a result page. And in google we have corresponding
keyword **intitle, allintitle, intext, allintext and filetype** to achieve these goals respectively.

- ### title
Search pages whose titles matching some keyword. 

- #### intitle
For example, we wanna search pages whose titles containing the ***zju*** keyword, we can do like this:

![intitle](./pictures/intitle.png)

And we can check the html source the see whether the title truly contains the ***zju*** keyword, as we can see the following 
picture, it does.

![intitle_html_source](./pictures/intitle_html_source.png)

**Notice: the words are case-insensitive.**

- #### allintitle
As I mentioned earlier, the operators prefixed with **all** require all the keywords exist simultaneously.

For example, if we wanna search pages whose titles containing the ***zju*** keyword, we can do like this:

![allintitle](./pictures/allintitle.png)

Similarly, we can check the html source shown below:

![allintitle_html_source](./pictures/allintitle_html_source.png)

- ### intext
Search for body part of a html page.

For example, we wanna search pages whose body contains ***google search skills***, we can write this:

![intext_example](./pictures/intext_example.png)

- ### allintext
You may notice that I also visited the fourth result in the above picture. And I found that the fourth 
doesn't contain the ***skills*** keyword, this is not surprising, for **intext** only require at least
one of the keyword.

If we want to body of pages contain all the three keywords, we can use **allintext**:

![allintext_example](./pictures/allintext_example.png)

And if we want the three keywords contained in body of pages continuously, we can use double quotes, which will
be introduced later:

![intext_with_double_quotes](./pictures/intext_with_double_quotes.png)

- ### filetype 
Find and download different kinds of documents.

For example, we wanna search some pdf files which contain the **javascript** keyword, we would type
search like this:

![after_use_filetype](./pictures/after_use_filetype.png)

but if we don't use the filetype operator and just type **javascript pdf**, then we are likely not get expected results:

![before_use_filetype](./pictures/before_use_filetype.png)


- ## others
There are some operators can be used both in location-directed and content-directed search, like **minus sign** and
**double quotes**.

- ### minus sign
Eliminate irrelevant results.
- ### double quotes,
Search an exact phrase.


# Caveats
> 
> - every word in a query matters
> - word order matters
> - words are case-insensitive
> - never trust one source



# resources
For more advanced search skills, you can visit the following two links.
- [Search Smarter: 30+ Google Search Tricks You Might Not Already Know][1](blog)
- [Google Search Education][2](videos)


[1]:https://zapier.com/blog/advanced-google-search-tricks
[2]:https://www.google.com/intl/en-us/insidesearch/searcheducation/
