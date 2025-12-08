# arthurfritz.net

A lightweight personal page with a single focus: daily inspiration and a clean layout.

- **Homepage:** simple introduction with a quick link to the quotes.
- **Quotes:** shows a new quote every day, with a live feed and offline fallback list.

## Deployment

Deployments run automatically via the GitHub Actions workflow in `.github/workflows/main.yml`. Every push to the `work` branch
(and `main` for compatibility) triggers an SFTP upload to the remote path defined in the `Pfad` repository secret, using the
`USER`, `PASSWORD`, and `HOST` secrets for authentication. To confirm a deployment or troubleshoot missing updates:

1. Verify the required secrets (`USER`, `PASSWORD`, `HOST`, `Pfad`) are set in the repository.
2. Push commits to the `work` branch so the workflow can run; check the Actions tab for deployment logs and errors.
3. Once the job succeeds, refresh the site (hard refresh with Ctrl+F5) to bypass cached assets.

No manual upload is needed—the workflow handles publishing to the configured webspace automatically.
