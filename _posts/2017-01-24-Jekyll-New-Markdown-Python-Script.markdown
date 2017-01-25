---
layout:     post
title:      Jekyll New Markdown Python Script
date:       2017-01-24 19:19:51
tags:       jekyll coding python scripts
---


If you are using Jekyll to post on your blog its to annoying to put date on file name and inside the file. So here's the simple way to do it. 
<!--break-->

{% highlight python %}
#new_post.py

from datetime import datetime

TEMPLATE = """\
---
layout:     post
title:      {0}
date:       {1}
tags:       {2}
---

"""

if __name__ == "__main__":

    title = raw_input("Title:\n")
    categories = raw_input("Categories:\n")

    timestamp = datetime.today().strftime("%Y-%m-%d %H:%M:%S")
    datestamp = datetime.today().strftime("%Y-%m-%d")

    file_name = datestamp + "-" + 
        "-".join(title.split(" ")) + ".markdown"
    
    with open(file_name, "w+") as file:
        file.write(TEMPLATE.format(title, timestamp, categories))
{% endhighlight %}

Just execute with `python new_post.py` in your `_posts` directory. It'll prompt you for a `title` and `categories` and then save all of that information, along with the current date/time, into a handy markdown file. Now you can create a new markdown file in a few seconds flat!