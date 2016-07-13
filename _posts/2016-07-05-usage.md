---
title: Usage
layout: post
permalink: /usage/
background: '#0a5'

slides:
 - title: Where are these slides?
   slide-data: You will find all these slides in the Front Matter of respective posts. Search inside <strong>_posts</strong> folder.
     
 - title: How to edit them?
   slide-data: All slides are mentioned under <strong>"slides:"</strong> in every post. Change its content for your needs.
   
 - title: Choose a theme!
   slide-data: Choose a theme using one of these in the Front Matter. <strong>black, white, league, sky, beige, simple, serif, blood(default), night, moon, solarized</strong>.<pre><code>
       
                -&nbsp;title:&nbsp;Some title
            
                &nbsp;&nbsp;slide-data:&nbsp;some data
                 
                &nbsp;&nbsp;theme:&nbsp;white
                 </code></pre>
   
 
 - title: Add background color!
   slide-data: Use <strong>background:</strong> attribute on a slide to change its backround color.<pre><code>
       
                -&nbsp;title:&nbsp;Some title
            
                &nbsp;&nbsp;slide-data:&nbsp;some data
                 
                &nbsp;&nbsp;background:&nbsp;'#0a5'
                 </code></pre>
   background: '#3498db'
   
 - title: Add a background image!
   slide-data: Mention <strong>image:</strong> attribute with complete path of the image in Front Matter for the particular slide. <pre><code>image:&nbsp;'/images/image-1.jpg'</code></pre>
   image: '/slides/images/rail.jpg'
   
 - title: Many more data types..
   slide-data: Checkout <a href="http://webjeda.com/slides/demo/">demo</a> page for more data types.
   
 - title: Download!
   slide-data: Visit the <a href="https://github.com/sharu725/slides">project page</a> or directly <a href="https://github.com/sharu725/slides/archive/master.zip">download</a>.

---

{% for slide in page.slides %}                 
<section data-background="{% if slide.image %}{{slide.image}}{% elsif slide.background %}{{slide.background}}{% else %}{{page.background}}{% endif %}">
        <h1>{{slide.title}}</h1>{{ slide.slide-data }}

</section>               
{% endfor %}
    
