---
layout: post
title: "在Jekyll中使用kramdown的toc生成文章目录"
date: 2020-03-16 13:32:20 +0300
description: 在Jekyll（+Github Pages）博客中使用默认的kramdown编辑器自带的toc目录生成功能生成markdown的目录 # (optional)
img:  # Add image post (optional)
tags: [kramdown,Jekyll,toc] 
---
<strong>Table of Contents</strong>

1. The generated Toc will be an ordered list
{:toc} 

kramdown支持自动生成目录。 只需将参考名称“ toc”分配给有序列表或无序列表，该列表将被实际目录替换，如果将“ toc”应用于无序列表则将其呈现为嵌套无序列表，否则将其呈现为嵌套有序列表。 应用于原始列表的所有属性也将应用于生成的TOC列表，如果未设置ID，则它将获得markdown-toc的ID。

设置auto_ids选项时，所有标头都将显示在目录中，因为它们都具有ID。 将类名称“ no_toc”分配给标题以将其从目录中排除。[<官方文档>](https://kramdown.gettalong.org/converter/html.html#toc)

# toc目录的使用

在Jekyll博客的每篇文章开头加上下方的特定代码，即可实现文章目录自动生成

生成无序列表形式的目录：

```markdown
<strong>Table of Contents</strong>
- this unordered seed list will be replaced by toc as unordered list
{:toc} 
```

生成有序列表形式的目录（实践证明这样写并不能正确生成有序目录，原因未知）：

```markdown
<strong>Table of Contents</strong>
1. The generated Toc will be an ordered list
{:toc}
```

如果不想特定标题出现在目录中，可以使用`{:.no_toc}`，如下所示：

```markdown
# 这里是标题，加上下方的“{:.no_toc}”后此标题将不会生成到目录中
{:.no_toc}
```

# 参数配置

在_config.yml文件中，可以配置一些参数：

```
markdown: kramdown     # 指定markdown编辑器
kramdown:
  toc_levels: "1,2"    # 要通过toc指令生成目录的标题级别，例如："1,3"意味着只有h1、h3标题会生成到目录中
```


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
