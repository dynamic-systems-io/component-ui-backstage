# component-developer-portal

Custom developer portal application image for `development-system` (Backstage-based).

## Includes

- GitHub auth backend provider module
- Catalog ingestion for dynamic-systems-io component repositories
- Kubernetes/Argo-ready backend config via app-config files

## Local build

```bash
cd /workspace/component-developer-portal
yarn install
yarn --cwd packages/backend build-image
```

## Developer portal OAuth callback URL

Configure GitHub OAuth app callback URL as:

`http://backstage.localhost:8080/api/auth/github/handler/frame`
