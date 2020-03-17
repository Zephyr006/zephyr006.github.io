---
layout: post
title: "在jekyll中使用kramdown的toc生成文章目录"
date: 2020-03-16 13:32:20 +0300
description: 在Jekyll（+Github Pages）博客中使用默认的kramdown编辑器自带的toc目录生成功能生成markdown的目录 # (optional)
img:  # Add image post (optional)
---
**Table of Contents**
{:.no_toc}
- this unordered seed list will be replaced by toc as unordered list
{:toc} 

# 项目部署
项目使用`Jekyll • 简单静态博客网站生成器`搭建，并且markdown编辑器使用`kramdown`
https://kramdown.gettalong.org/converter/html.html#toc


You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. You can rebuild the site in many different ways, but the most common way is to run `jekyll serve`, which launches a web server and auto-regenerates your site when a file is updated.

To add new posts, simply add a file in the `_posts` directory that follows the convention `YYYY-MM-DD-name-of-post.ext` and includes the necessary front matter. Take a look at the source for this post to get an idea about how it works.

Jekyll also offers powerful support for code snippets:

~~~java
public static void main(String[] args) {
    System.out.println("1233");
}
~~~

{% highlight ruby %}
def print_hi(name)
  puts "Hi, #{name}"
end
print_hi('Tom')
#=> prints 'Hi, Tom' to STDOUT.
{% endhighlight %}
{% highlight java %}
public static void main(String[] args) {
    System.out.println("1233");
}
{% endhighlight %}

Check out the [Jekyll docs][jekyll-docs] for more info on how to get the most out of Jekyll. File all bugs/feature requests at [Jekyll’s GitHub repo][jekyll-gh]. If you have questions, you can ask them on [Jekyll Talk][jekyll-talk].

[jekyll-docs]: https://jekyllrb.com/docs/home
[jekyll-gh]:   https://github.com/jekyll/jekyll
[jekyll-talk]: https://talk.jekyllrb.com/
