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
        Oscar (he/him) is an Anthrozoology M.S. student at Canisius College and software developer. He plans to graduate in 2024 and is looking for PhD positions related to animal ethics, conservation, and longtermism. He is interested in the intersection of technology and animal studies and wants to find ethical, respectful, applications for technology in nonhuman animals’ lives.
        <h3> Contact </h3>
        <ul class="links">
            <li>
                <span class="c-title"> Email: </span> courchao@canisius.edu
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