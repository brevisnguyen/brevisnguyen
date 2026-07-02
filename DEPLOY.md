# Deploy GitHub Profile README

This guide publishes the profile page from this project to your GitHub profile.

## 1) Prepare your profile repository

1. Sign in to GitHub.
2. Create a new public repository named exactly as your username.
   - Example: if your username is `brevisnguyen`, the repository must be `brevisnguyen/brevisnguyen`.
3. Do not initialize it with another README if you want a clean push from this project.

## 2) Customize content (optional)

The starter files are already configured for `brevisnguyen`.
If you clone this template for another account, update username and profile links in `README.md` and `.github/workflows/snake.yml`.

Optional cleanup:
- Remove sections you do not use.
- Adjust badges to match your real stack.

## 3) Push this project to GitHub

Run these commands from `~/Documents/project/brevis`:

```bash
git add .
git commit -m "Create dark modern GitHub profile README"
git branch -M main
git remote add origin https://github.com/brevisnguyen/brevisnguyen.git
git push -u origin main
```

If remote already exists:

```bash
git remote set-url origin https://github.com/brevisnguyen/brevisnguyen.git
git push -u origin main
```

## 4) Verify profile rendering

1. Open `https://github.com/brevisnguyen`.
2. Confirm the README appears on top of the profile.
3. Wait a few minutes for stats cards to refresh.

## 5) Optional snake animation setup

After first push:

1. Open repository `Settings` -> `Actions` -> `General`.
2. Ensure actions are allowed.
3. Open the `Generate Contribution Snake` workflow and run it once with `Run workflow`.
4. Verify this URL resolves:
   - `https://raw.githubusercontent.com/brevisnguyen/brevisnguyen/output/github-contribution-grid-snake-dark.svg`

## Troubleshooting

- Stats cards not showing:
  - Check that profile links use `brevisnguyen`.
  - Retry later if Vercel-hosted card services are temporarily rate-limited.
- Snake image not showing:
  - Confirm workflow completed successfully.
  - Confirm `output` branch was created by workflow.
- README not visible on profile:
  - Repository name must match exact GitHub username.
  - Repository must be public.

