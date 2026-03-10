# GitHub Secrets Required

Create these repository secrets in GitHub:

1. `METRICS_TOKEN`
2. `STEAM_TOKEN`
3. `STEAM_USER_ID`

## What each secret is for

- `METRICS_TOKEN`
  - Used by `lowlighter/metrics` to fetch GitHub data and write SVG output.
  - Referenced in:
    - `.github/workflows/blank.yml`
    - `.github/workflows/metrics.yml`

- `STEAM_TOKEN`
  - Steam Web API key used by the Steam plugin in `metrics.yml`.
  - Referenced in:
    - `.github/workflows/metrics.yml`

- `STEAM_USER_ID`
  - Steam user ID (numeric SteamID64) for the Steam plugin in `metrics.yml`.
  - Referenced in:
    - `.github/workflows/metrics.yml`

## How to add secrets

1. Open your repo on GitHub.
2. Go to `Settings` -> `Secrets and variables` -> `Actions`.
3. Click `New repository secret`.
4. Add each secret name/value above.
