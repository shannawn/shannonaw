------
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta name="description" content="brain doodles"/>
    <meta property="og:title" content="brain doodles">
    <title>brain doodles</title>
    <link href="https://fonts.googleapis.com/css2?family=Work+Sans:wght@300;400;500&display=swap" rel="stylesheet">
    <link rel="stylesheet" type="text/css" href="./brain-doodles/stylesheet.css">
    <link rel="apple-touch-icon" sizes="57x57" href="../shortcut_icons/apple-icon-57x57.png">
    <link rel="apple-touch-icon" sizes="60x60" href="../shortcut_icons/apple-icon-60x60.png">
    <link rel="apple-touch-icon" sizes="72x72" href="../shortcut_icons/apple-icon-72x72.png">
    <link rel="apple-touch-icon" sizes="76x76" href="../shortcut_icons/apple-icon-76x76.png">
    <link rel="apple-touch-icon" sizes="114x114" href="../shortcut_icons/apple-icon-114x114.png">
    <link rel="apple-touch-icon" sizes="120x120" href="../shortcut_icons/apple-icon-120x120.png">
    <link rel="apple-touch-icon" sizes="144x144" href="../shortcut_icons/apple-icon-144x144.png">
    <link rel="apple-touch-icon" sizes="152x152" href="../shortcut_icons/apple-icon-152x152.png">
    <link rel="apple-touch-icon" sizes="180x180" href="../shortcut_icons/apple-icon-180x180.png">
    <link rel="icon" type="image/png" sizes="192x192"  href="../shortcut_icons/android-icon-192x192.png">
    <link rel="icon" type="image/png" sizes="32x32" href="../shortcut_icons/favicon-32x32.png">
    <link rel="icon" type="image/png" sizes="96x96" href="../shortcut_icons/favicon-96x96.png">
    <link rel="icon" type="image/png" sizes="16x16" href="../shortcut_icons/favicon-16x16.png">
    <link rel="manifest" href="../shortcut_icons/manifest.json">
    <meta name="msapplication-TileColor" content="#ffffff">
    <meta name="msapplication-TileImage" content="../ms-icon-144x144.png">
    <meta name="theme-color" content="#ffffff">
  </head>
  <body>
    <header>
      <h1>brain doodles</h1>
    </header>
    <main>
      {% assign doclist = site.pages | sort: 'url'  %}
        <div class="text-container-left">
        {% for doc in doclist %}
          {% if doc.name != 'index.md' and doc.name contains '.md' %}
            <p>
              <a href="{{ site.baseurl }}{{ doc.url }}">{{ doc.title }}</a>
            </p>
          {% endif %}
        {% endfor %}
        </div> 
    </main>
  </body>
</html>
