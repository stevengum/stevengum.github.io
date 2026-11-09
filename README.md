# stevengum97.github.io
Demo/hosting page for various projects.

## Local development

Requires Ruby 3.3 and Bundler.

```sh
bundle install
bundle exec jekyll serve
```

Then open http://localhost:4000.

## Deployment

In **Settings → Pages → Build and deployment**, set **Source** to
**GitHub Actions**. The Pages workflow builds the site with Jekyll and publishes it on pushes to
`master` and can also be run manually.

Deployments share the `pages` concurrency group and wait for an active workflow
run to finish rather than canceling it. If Pages reports an existing deployment
in progress, let that deployment finish or cancel its originating run before
retrying. The workflow cannot clear an already-stuck Pages deployment.
