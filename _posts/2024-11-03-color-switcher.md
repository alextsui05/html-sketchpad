<html lang="{{ site.lang | default: "en-US" }}">
  <head>
    <meta name="viewport" content="width=device-width, initial-scale=1">
    <meta charset="utf-8">
    <title>{{ page.title }} - {{ site.title }}</title>
    <script type="text/javascript" src="{{ "/assets/js/main.js" | relative_url }}"></script>
    <link rel="stylesheet" href="{{ "/assets/css/main.css" | relative_url }}">
  </head>
  <body>
    <div class="py-24 max-w-4xl mx-auto">
      {% include navbar.html %}
      <div>
        <h1>Color switcher</h1>
        <div>
          <button class="btn" data-color-toggle>
            {{ page.slug }}
          </button>
        </div>
        <h1>String compression</h1>
        <div>
          <input type="text">
          <button>Submit</button>
        </div>
      </div>
    </div>
  </body>
  <script type="text/javascript">
    document.addEventListener('DOMContentLoaded', () => {
      const colorToggle = document.querySelector('[data-color-toggle]');
      if (colorToggle) {
        colorToggle.addEventListener('click', () => {
          colorToggle.classList.toggle('toggled');
        });
      }
    });
  </script>
</html>
