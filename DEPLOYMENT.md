# GitHub Pages deployment

The active GitHub Actions workflow is located at:

```text
.github/workflows/deploy.yml
```

The `.github` directory is hidden by default on Linux and macOS. To confirm it exists, run:

```bash
ls -la
ls -la .github/workflows
```

After pushing the complete project to GitHub:

1. Open **Settings > Pages** in the repository.
2. Select **GitHub Actions** under **Source**.
3. Open the **Actions** tab and select **Build and Deploy**.
4. Use **Run workflow** if a deployment did not start automatically.

When copying files with a graphical file manager, make sure hidden files are visible so that the `.github` directory is copied too.

