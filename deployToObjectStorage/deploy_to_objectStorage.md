## PREREQUISITES
- Go to GitHub repository settings.
- On the left menu, select **Secrets** under **Actions**.
- Set the following secrets:
  - `PROD_GOOGLE_MAP_KEY`
  - `PROD_GOOGLE_API_KEY`
  - `VITE_PROD_URL`
  - `VITE_BASE_URL`
  - `VITE_DEFAULT_LOCALE`
  - `VITE_FALLBACK_LOCALE`
  - `VITE_SUPPORTED_LOCALES`
  - `PROD_NAFADH_URL`
  - `PROD_NAFADH_APP_ID`
  - `PROD_NAFADH_APP_KEY`
  - `OBS_ENDPOINT`
  - `OBS_BUCKET`
  - `OBS_ACCESS_KEY`
  - `OBS_SECRET_KEY`
  - `SLACK_WEBHOOK_URL` (Optional for notifications)

## SETUP
1. Create a directory named `.github/workflows/` in your repository.
2. In that directory, create a file with a `.yml` extension (e.g., `deploy.yml`).
3. Place the workflow configuration in the `.yml` file.
4. The workflow will trigger on each push to the `dev` branch.
5. Ensure that the deployment script (`deploy.yml`) is properly configured for your project's specific needs.

## WORKFLOW DESCRIPTION
1. **Checkout Repository:** Checks out the code from the repository.
2. **Set up Node.js:** Sets up the Node.js environment.
3. **Cache Node Modules:** Caches Node.js modules to speed up subsequent builds.
4. **Install Dependencies:** Installs the project's dependencies.
5. **Build Vue Project:** Builds the Vue.js project.
6. **Deploy to OBS:** Deploys the built project to Huawei Cloud Object Storage (OBS).
7. **Notify Slack on Success:** Sends a Slack notification if the deployment succeeds.
8. **Notify Slack on Failure:** Sends a Slack notification if the deployment fails.
