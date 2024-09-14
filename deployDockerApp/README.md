## PREREQUISITES:
- Go to AWS settings.
- On the left menu, select **Secrets** under **Actions**.
- Set the following secrets in your GitHub repository:
  - `AWS_ACCESS_KEY_ID`
  - `AWS_SECRET_ACCESS_KEY`
  - `AWS_ACCOUNT_ID`
  - `EC2_INSTANCE_HOST`
  - `EC2_USER`
  - `EC2_SSH_KEY`
  - `SLACK_WEBHOOK_URL` (Optional)

## SETUP:
1. Make a directory named `.github/workflows/`.
2. In that directory, create a file with a `.yml` extension (e.g., `deploy.yml`).
3. Place the workflow configuration in the `.yml` file.
4. This will run on every push to the `main` branch.
