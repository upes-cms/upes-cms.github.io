# GitHub Pages deployment

## Required repository name

This package is configured as the root website for the `UPES-CMS` organization. The repository must be named exactly:

```text
upes-cms.github.io
```

This publishes the site at:

```text
https://upes-cms.github.io
```

If the existing repository is named `webpage`, open **Settings > General > Repository name**, rename it to `upes-cms.github.io`, and confirm the rename.

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

The Jekyll configuration uses an empty `baseurl` because this is an organization-root website. Do not change it to `/webpage`.

When copying files with a graphical file manager, make sure hidden files are visible so that the `.github` directory is copied too.
