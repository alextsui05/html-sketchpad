# html-sketchpad

Just a sketchpad of HTML, CSS (Tailwind), and JS

# Local dev

Since `_config.yml` is configured with Github pages in mind, running Jekyll locally will not have proper pathing.
We can override this by specifying another config file like so:

```
bundle exec jekyll serve --config _config.yml,dev.yml
```
