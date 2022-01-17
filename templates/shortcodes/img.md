{% set meta = get_image_metadata(path=path) %}

{% if width %}
{% set _width = width %}
{% set scale = _width / meta.width %}
{% else %}
{% set _width = config.extra.img_post_width %}
{% if _width > meta.width %}
{% set _width = meta.width %}
{% endif %}
{% set scale = _width / meta.width %}
{% endif %}

{% if height %}
{% set _height = height %}
{% else %}
{% set _height = meta.height * scale | round | int %}
{% endif %}

{% set img = resize_image(path=path, width=_width, height=_height, op="fill") -%}
![some mig]({{ img.url }})
