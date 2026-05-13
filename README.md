# component-ui-backstage

Custom Backstage application image for `development-system`.

## Includes

- GitHub auth backend provider module
- Catalog ingestion for dynamic-systems-io component repositories
- Kubernetes/Argo-ready backend config via app-config files

## Local build

```bash
cd /workspace/component-ui-backstage
yarn install
yarn --cwd packages/backend build-image
```

## OAuth callback URL

Configure GitHub OAuth app callback URL as:

`http://backstage.localhost:8080/api/auth/github/handler/frame`
