# html-sketchpad

Just a sketchpad of HTML, CSS (Tailwind), and JS

# Local dev

`package.json` provides a script to run Jekyll server with a local config:

```
yarn dev
```

It runs the following command:

```
bundle exec jekyll serve --config _config.yml,dev.yml
```

Since `_config.yml` is configured with Github pages in mind, running Jekyll locally will not have proper pathing.
The `dev.yml` nulls out the url and baseurl so pages are accessible.
