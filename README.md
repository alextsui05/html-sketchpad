# alextsui05.github.io

This is the source code for my personal developer webpage hosted at https://alextsui05.github.io

It is built with Jekyll and Tailwind.
Github Actions handles the deploy and is triggered by a push to the main branch.
Feel free to clone it as a starting point.
Alternatively, I have some starter code with some more info in another repository: https://github.com/alextsui05/jekyllwind-test/

# Local dev

Since `_config.yml` is configured with Github pages in mind, running Jekyll locally will not have proper pathing.
We can override this by specifying another config file like so:

```
bundle exec jekyll serve --config _config.yml,dev.yml
```
