---
layout: mypost
title: 友情链接
---

友链需要满足以下条件：

 - 独立博客，独立域名
 - 全站 HTTPS
 
以及，这只是基本要求，但是本站不接受友链申请，如果您的博客或者您和我很熟悉，我会自己加上作为收藏备份，主动要求加友链的一律拒绝。

```
名称：{{ site.title }}
描述：{{ site.description }}
地址：{{ site.domainUrl }}{{ site.baseurl }}
头像：{{ site.domainUrl }}{{ site.baseurl }}/static/files/logo.jpg
```

<ul>
  {%- for link in site.links %}
  <li>
    <p><a href="{{ link.url }}" title="{{ link.desc }}" target="_blank" >{{ link.title }}</a></p>
  </li>
  {%- endfor %}
</ul>
