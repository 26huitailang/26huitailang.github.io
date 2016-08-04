---
layout: page
title: Aloha!
tagline: Welcome to Peter's blog
---
{% include JB/setup %}

本站由Jekyll和Github Pages建成，主要使用了Jekyll Bootstrap的模板。

以下为本站**正式内容**：

## Recent

最近，看完Wes McKinney的《利用Python进行数据分析》这本书后，自己动手敲了一遍ipynb，然后去kaggle上找了一个关于Kobe的入门数据练习，还是觉得基础不是很扎实，所以在Udemy上找了一个课程来学习，最近应该会更新一些ipynb，也方便还没入门的学习者了解到基础。

## Posts

    2016-Aug-02之前的文章是模板，暂时未去掉。

<ul class="posts">
  {% for post in site.posts %}
    <li><span>{{ post.date | date_to_string }}</span> &raquo; <a href="{{ BASE_PATH }}{{ post.url }}">{{ post.title }}</a></li>
  {% endfor %}
</ul>

## To-Do

- [ ] 未来可能会增加一个多说评论，但是github下面交流比较集中一点，后续有需要再更新吧。
- [ ] 搜索功能暂时不能用
- [ ] 顺便推荐一个漂亮的博客[HUX](http://huangxuan.me/about/)
- [ ] 首页增加Tags，方便筛选

## Suggestion

如果对于我的学习和页面有什么建议，可以去我的github:[26huitailang](https://github.com/26huitailang/26huitailang.github.io/issues)上提出，谢谢！


