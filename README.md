# stevengum97.github.io
Demo/hosting page for various projects.

## Deployment

In **Settings → Pages → Build and deployment**, set **Source** to
**GitHub Actions**. The Pages workflow publishes the static site on pushes to
`master` and can also be run manually.

Deployments share the `pages` concurrency group and wait for an active workflow
run to finish rather than canceling it. If Pages reports an existing deployment
in progress, let that deployment finish or cancel its originating run before
retrying. The workflow cannot clear an already-stuck Pages deployment.
