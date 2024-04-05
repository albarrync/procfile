---
# Feel free to add content and custom Front Matter to this file.
# To modify the layout, see https://jekyllrb.com/docs/themes/#overriding-theme-defaults

layout: home
---

## Hey, where's my Procfile?
Most visits to this page are from folks who are simply trying to view a local Procfile. If this is you, have a wonderful day 👋

## What is a Procfile?
A Procfile contains instructions for a web server that details services and configurations on boot. It's common practice to maintain Procfiles for different environments, so a project may have a `Procfile.dev` and a standard `Procfile` - the latter of which would serve as instructions for a production environment, and the former serving local development. They're common in Rails and Node apps.

Sometimes, folks click on a link to their local Procfile.dev, and accidentally open a browser, which is why this site exists.

## Example of a Procfile
```
# Procfile.dev

web: bin/rails server -p 3000
css: bin/rails tailwindcss:watch
redis: redis-server
sidekiq: bundle exec sidekiq -C config/sidekiq.yml
```

This file runs a puma webserver, a Tailwind watcher, Redis, and Sidekiq all with one command.
Much better than running all these services in their own terminal windows~

## Further Reading
[Rails Procfiles](https://railsnotes.xyz/blog/procfile-bin-dev-rails7)

[Heroku Procfiles](https://devcenter.heroku.com/articles/procfile)

## Cheers!
