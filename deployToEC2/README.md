## PREREQUISITES:
- Go to GitHub repository settings.
- On the left menu, select **Secrets** under **Actions**.
- Set the following secrets:
  - `STAGE_SSH_USERNAME`
  - `STAGE_SSH_HOST`
  - `STAGE_SSH_KEY`
  - `SLACK_WEBHOOK_URL` (Optional)

## SETUP:
1. Create a directory named `.github/workflows/` in your repository.
2. In that directory, create a file with a `.yml` extension (e.g., `deploy.yml`).
3. Place the workflow configuration in the `.yml` file.
4. This workflow will run on every push to the `dev` branch.
5. Ensure the deployment script (`deploy.yml`) is properly configured to match your server setup.
