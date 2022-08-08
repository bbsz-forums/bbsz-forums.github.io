# My Indie Developer Game Devlogs

<h4>In here you should be able to see all of my indie dev game devlogs that I've made on this website. These Posts includes my status updates, datapack updates, mod updates, and so on.</h4>

{% for category in site.categories %}
  <h2>{{ category[0] }}</h2>
  <ul>
    {% for minecraft-datapacks-devlogs in category[1] %}
      <li><a href="{{ minecraft-datapacks-devlogs.url }}"><i>{{ minecraft-datapacks-devlogs.date }}</i> <b>{{ minecraft-datapacks-devlogs.title }}</b></a></li>
    {% endfor %}
  </ul>
{% endfor %}

