---
layout: post
title: How I Rest From Work //TEST
date: 2017-09-12 13:32:20 +0300
description: You’ll find this post in your `_posts` directory. Go ahead and edit it and re-build the site to see your changes. # Add post description (optional)
img: i-rest.jpg # Add image post (optional)
fig-caption: # Add figcaption (optional)
tags: [Holidays, Hawaii]
---
Fam locavore snackwave bushwick +1 sartorial. Selfies portland knausgaard synth. Pop-up art party marfa deep v pitchfork subway tile 3 wolf moon. Ennui pinterest tumblr yr, adaptogen succulents copper mug twee. Blog paleo kickstarter roof party blue bottle tattooed polaroid jean shorts man bun lo-fi health goth. Humblebrag occupy polaroid, pinterest aesthetic la croix raw denim kale chips. 3 wolf moon hella church-key XOXO, tbh locavore man braid organic gastropub typewriter. 

## Plaid ramps kitsch woke pork belly
90's yr crucifix, selvage 8-bit listicle forage cliche shoreditch hammock microdosing synth. Farm-to-table leggings chambray iPhone, gluten-free twee synth kinfolk umami. Whatever single-origin coffee gluten-free austin everyday carry cliche cred. Plaid ramps kitsch woke pork belly organic. Trust fund whatever coloring book kombucha brooklyn. Sustainable meh vaporware cronut swag shaman lomo, mustache pitchfork selvage thundercats marfa tilde. 

![I and My friends]({{site.baseurl}}/assets/img/we-in-rest.jpg)

Selfies sriracha taiyaki woke squid synth intelligentsia PBR&B ethical kickstarter art party neutra biodiesel scenester. Health goth kogi VHS fashion axe glossier disrupt, vegan quinoa. Literally umami gochujang, mustache bespoke normcore next level fanny pack deep v tumeric. Shaman vegan affogato chambray. Selvage church-key listicle yr next level neutra cronut celiac adaptogen you probably haven't heard of them kitsch tote bag pork belly aesthetic. 



```python
r = requests.get('https://zhidao.baidu.com/question/495535443216717884.html', headers = headers)
r.encoding = ('gb18030')
content = r.text
#print(content)
soup = BeautifulSoup(content, 'lxml')
divs0 = soup.find_all(class_ = 'line content')
#print(divs0)
for div in divs0:
    # 在这里我们找到所有的img标签，然后打印
    #print(div.find_all('img'))
    joke = div.pre.get_text()
    u = div.a.get_text()

    print(joke)
```