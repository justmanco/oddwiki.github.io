# {{ include.item.name }}

> {{ include.item.quote }}

{{ include.item.summary }}

{% include toc.html %}

# Biology
{{ include.item.biology }}

# Background
{{ include.item.background }}

# Notable Individuals
{% for individual in include.item.notable-individuals %}
  * {{ individual }}
{% endfor %}

# Appears In
{% for appearance in include.item.appears-in %}
  * {{ appearance }}
{% endfor %}

# Trivia
{{ include.item.trivia }}

# Gallery
{% for image in include.item.gallery %}
  ![]({{ image.image-url }})

  {{ image.description }}
{% endfor %}

# References
{% for reference in include.item.references %}
  * {{ reference }}
{% endfor %}
