# My Posts

<h4>In here you should be able to see all of my posts that I've made on this website. These Posts includes my status updates, datapack updates, mod updates, and so on.</h4>

{% for category in site.categories %}
  <h2>{{ category[0] }}</h2>
  <ul>
    {% for post in category[1] %}
      <li><a href="{{ post.url }}"><i>{{ post.date }}</i> <b>{{ post.title }}</b></a></li>
    {% endfor %}
  </ul>
{% endfor %}

