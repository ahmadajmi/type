---
layout: post
title: Welcome to Jekyll!
featured: true
tags: [frontpage, jekyll, blog]
image: '/images/posts/image18.jpeg'
---

You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

{% highlight bash %}
#!/bin/bash

IP_ADDRESS='192.241.2.10'

cd /Users/ahmadajmi/www/aspirethemes/wp-content/themes/

zip -r theme_name.zip theme_name -x *node_modules* *git* *.DS_Store*

echo '===>> Zipped'

scp theme_name.zip root@$IP_ADDRESS:/var/www/html/wp-content/themes/

echo '===>> Pushed'

ssh -t -t root@$IP_ADDRESS << EOT

cd /var/www/html/wp-content/themes/

unzip -o theme_name.zip

echo '===>> Un Zipped'

exit 1

EOT
{% endhighlight %}

{% highlight bash %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: http://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/