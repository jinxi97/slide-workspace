# Deploy to Cloudflare Pages

## 1. Create the Project (one-time)

```bash
CLOUDFLARE_API_TOKEN=<your-token> wrangler pages project create <project-id> --production-branch main
```

## 2. Deploy

```bash
CLOUDFLARE_API_TOKEN=<your-token> wrangler pages deploy . --project-name <project-id>
```

Your site will be live at:
```
https://<deployment-id>.<project-id>.pages.dev
```

> For future deploys, skip step 1 and run step 2 only.
