# introduction
This repo is used to record some search skills for googling.

# basic
Almost each result returned by google has three parts, and they are the **title**, **url** and **body**.
As the following picture shows, the content in **red**, **light green** and **blue** box is **title**, **url** and **body** part respectively.

![three_parts_of_result](./pictures/three_parts_of_result.png)

# advanced search skills

The skills to be introduced may be roughly divided into three categories: location-directed, content-directed and others.

## 1. location-directed 
In this way, we can filter pages according the location. specifically, we can use the site and url of a page
to control the location.

### 1.1 site
By its very name, we can tune our search to make result limited to some specific location and by location, 
I mean the domain of web pages. In google, we can use **site** keyword to achieve this goal.

For example, we wanna search pages which contain **javascript prototype**, we can type search like this:

![before_use_site_keyword](./pictures/before_use_site_keyword.png)

As we can see in the picture above, the result pages do contain **javasript and/or prototype**, but 
we now want pages only from some domain, say ***stackoverflow.com***, for pages from this domain are more likely
have high-quality contents we may need, so we can tune our search like this:

![after_use_site_keyword](./pictures/after_use_site_keyword.png)

So the result pages now are all from the same domain of ***stackoverflow.com***.

### 1.2 url
We can further do something on the url of pages. And in google we have two related operators: inurl and allinurl.

#### 1.2.1 inurl

For example, we wanna pages whose urls contain **zju and/or cs** , so we can construct our search like this:

![inurl_example](./pictures/inurl_example.png)

#### 1.2.2 allinurl
The key difference between inurl and allinurl is that the latter one requires all the keywords be contained in url, while
the former require at least one of keywords represent in url. The following picture shows the result using **allinurl**:

![allinurl_example](./pictures/allinurl_example.png)

As far as I know, we can tune the site and url of pages to make result pages more closer to what we expect as to the 
location of pages.

## 2. content-directed 
In this way, we can tune our search according the title, body, filetype of a result page. And in google we have corresponding
keyword **intitle, allintitle, intext, allintext and filetype** to achieve these goals respectively.

### 2.1 title
Search pages whose titles matching some keyword. 

#### 2.1.1 intitle
For example, we wanna search pages whose titles contain the ***zju*** keyword, we can do like this:

![intitle](./pictures/intitle.png)

And we can check the html source the see whether the title truly contains the ***zju*** keyword, as we can see the following 
picture, it does.

![intitle_html_source](./pictures/intitle_html_source.png)

**Notice: the words are case-insensitive.**

#### 2.1.2 allintitle
As I mentioned earlier, the operators prefixed with **all** require all the keywords exist simultaneously.

For example, if we wanna search pages whose titles contain the ***zju*** keyword, we can do like this:

![allintitle](./pictures/allintitle.png)

Similarly, we can check the html source shown below:

![allintitle_html_source](./pictures/allintitle_html_source.png)

### 2.2 intext
Search for body part of a html page.

#### 2.2.1 intext
For example, we wanna search pages whose body contains ***google search skills***, we can write this:

![intext_example](./pictures/intext_example.png)

#### 2.2.2 allintext
You may notice that I also visited the fourth result in the above picture. And I found that the fourth 
doesn't contain the ***skills*** keyword, this is not surprising, for **intext** only require at least
one of the keyword.

If we want to body of pages contain all the three keywords, we can use **allintext**:

![allintext_example](./pictures/allintext_example.png)

And if we want the three keywords contained in body of pages continuously, we can use double quotes, which will
be introduced later:

![intext_with_double_quotes](./pictures/intext_with_double_quotes.png)

### 2.3 filetype 
Find and download different kinds of documents.

For example, we wanna search some pdf files which contain the **javascript** keyword, we would type
search like this:

![after_use_filetype](./pictures/after_use_filetype.png)

but if we don't use the filetype operator and just type **javascript pdf**, then we are more likely not to get expected results:

![before_use_filetype](./pictures/before_use_filetype.png)


## 3. others
There are some operators can be used both in location-directed and content-directed search, like **minus sign** and
**double quotes**.

### 3.1 minus sign
Eliminate irrelevant results.
### 3.2 double quotes
Search an exact phrase.
### 3.3 asterisk
Use an asterisk within quotes to specify unknown or variable words
> Here’s a lesser known trick: searching a phrase in quotes with an asterisk replacing a word will search all 
> variations of that phrase. It’s helpful if you’re trying to determine a song from its lyrics, but you couldn’t 
> make out the entire phrase (e.g. "imagine all the * living for today"), or if you're trying to find all forms 
> of an expression (e.g. "* is thicker than water").

# caveats
> 
> - every word in a query matters
> - word order matters
> - words are case-insensitive
> - never trust one source

# tips
- Keep in mind that we should tune our search for good result. So if you are not satisfied with the result returned, you can
try to tune the search until you find what is expected.

# resources
For more advanced search skills, you can visit the following two links.
- [Search Smarter: 30+ Google Search Tricks You Might Not Already Know][1](blog)
- [Google Search Education][2](videos)
- [20 Google Search Tips to Use Google More Efficiently][3](blog)

[1]:https://zapier.com/blog/advanced-google-search-tricks
[2]:https://www.google.com/intl/en-us/insidesearch/searcheducation/
[3]:https://www.lifehack.org/articles/technology/20-tips-use-google-search-efficiently.html
