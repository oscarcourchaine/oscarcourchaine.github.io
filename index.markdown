---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: default
---

<div class="flex-container">
    <div class="flex-child">
        <img class="mainphoto" src="../media/oscar.jpeg">
    </div>
    <div class="flex-child info">
        Oscar (he/him) is a software developer and recent graduate from Canisius University with his M.S. degree in Anthrozoology. He is interested in the intersection of animal studies and technology and wants to find ethical, respectful, applications for technology to improve nonhuman animals’ lives. He is now looking for PhD positions related to animal ethics, conservation philosophy, and the environmental humanities with a desired start date in 2025. 
        <h3> Contact </h3>
        <ul class="links">
            <li>
                <span class="c-title"> Email: </span> oscar.courchaine@gmail.com
            </li>
        </ul>
    </div>
</div>

<div class="feed">
<h2> Posts </h2>
<ul>
    {% for item in site.data.feed %}
        <li class="post">
            <span class="post-date"> {{ item.date }} </span>
            <span class="post-text"> {{ item.text }} </span>
            {% if item.image %}
                <img class="post-image" src="../media/{{ item.image }}">
            {% endif %}
        </li>
    {% endfor %}
</ul>
</div>