---
layout: article
titles:
  # @start locale config
  en      : &EN       Wiki
  en-GB   : *EN
  en-US   : *EN
  en-CA   : *EN
  en-AU   : *EN
  zh-Hans : &ZH_HANS 维基百科
  zh      : *ZH_HANS
  zh-CN   : *ZH_HANS
  zh-SG   : *ZH_HANS
  zh-Hant : &ZH_HANT 維基百科
  zh-TW   : *ZH_HANT
  zh-HK   : *ZH_HANT
  # @end locale config
key: page-wiki
permalink: /wiki
---

> 在维基百科查询你最需要的知识！

```
 __      __.__ __   .__                  .___.__        
/  \    /  \__|  | _|__|_____   ____   __| _/|__|____   
\   \/\/   /  |  |/ /  \____ \_/ __ \ / __ | |  \__  \  
 \        /|  |    <|  |  |_> >  ___// /_/ | |  |/ __ \_
  \__/\  / |__|__|_ \__|   __/ \___  >____ | |__(____  /
       \/          \/  |__|        \/     \/         \/ 
```

<ul class="listing">
{% for wiki in site.wiki %}
{% if wiki.title != "Wiki Template" %}
<li class="listing-item"><a href="{{ site.url }}{{ wiki.url }}">{{ wiki.title }}</a></li>
{% endif %}
{% endfor %}
</ul>

