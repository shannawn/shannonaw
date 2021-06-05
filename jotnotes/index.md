------
<html>
    <head>
        <title>Index of /thoughts/</title>
    </head>
    <body bgcolor="white">   
        {% assign doclist = site.pages | sort: 'url'  %}
    <ul>
       {% for doc in doclist %}
            {% if doc.name contains '.md' or doc.name contains '.html' %}
                <li><a href="{{ site.baseurl }}{{ doc.url }}">{{ doc.url | relative_url }}</a></li>
            {% endif %}
        {% endfor %}
    </ul> 
    </body>
</html>