# arthurfritz.net
Coding mit Arthur
Test fuer Aenderung MF
Meine ersten Teständerungen
UND WIEDER PAPA
und noch
und wiedet af

## Deployment

Deployments run automatically via the GitHub Actions workflow in `.github/workflows/main.yml`. Every push to the `work` branch
(and `main` for compatibility) triggers an SFTP upload to the remote path defined in the `Pfad` repository secret, using the
`USER`, `PASSWORD`, and `HOST` secrets for authentication. To confirm a deployment or troubleshoot missing updates:

1. Verify the required secrets (`USER`, `PASSWORD`, `HOST`, `Pfad`) are set in the repository.
2. Push commits to the `work` branch so the workflow can run; check the Actions tab for deployment logs and errors.
3. Once the job succeeds, refresh the site (hard refresh with Ctrl+F5) to bypass cached assets.

No manual upload is needed—the workflow handles publishing to the configured webspace automatically.

## Animated flower demo
Open `index.html` in any browser to see a lightweight animated flower built with pure HTML and CSS. The design keeps markup and animations simple so it runs smoothly even on weak computers.
