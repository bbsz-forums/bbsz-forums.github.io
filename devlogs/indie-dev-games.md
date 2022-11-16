# My Indie Developer Game Devlogs

<h4>In here you should be able to see all of my indie dev game devlogs that I've made on this website. These Posts includes my status updates, datapack updates, mod updates, and so on.</h4>

{% for category in site.categories %}
  <h2>{{ category[0] }}</h2>
  <ul>
    {% for indie_dev_games_devlogs in category[1] %}
      <li><a href="{{ indie_dev_games_devlogs.url }}"><i>{{ indie_dev_games_devlogs.date }}</i> <b>{{ indie_dev_games_devlogs.title }}</b></a></li>
    {% endfor %}
  </ul>
{% endfor %}

