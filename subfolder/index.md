# This is in a subfolder

Some text ...

<ul>
{% for member in site.data.members %}
  <li>
    <a href="https://github.com/{{ member.github }}">
      {{ member.name }}
    </a>
  </li>
{% endfor %}
</ul>


<ul>
{% for member in site.subfolder.data.members %}
  <li>
      {{ member.name }}, {{ member.born }}
  </li>
{% endfor %}
</ul>



<ul>
{% for member in site.data.subfolder.members %}
  <li>
      {{ member.name }}, {{ member.born }}
  </li>
{% endfor %}
</ul>


<ul>
{% for member in subfolder.data.members %}
  <li>
      {{ member.name }}, {{ member.born }}
  </li>
{% endfor %}
</ul>

{{ site }}