# Organization Description for eduTAP-eu

## Shared Renovate preset

[`renovate-config.json5`](renovate-config.json5) holds the Renovate rules every eduTAP repository wants:
digest-pinned GitHub Actions and images, grouped development tooling, weekly lock file maintenance, and
security updates labelled `security` (from GitHub's advisories and osv.dev). A repository opts in with

```json5
{ extends: ["github>edutap-eu/.github:renovate-config.json5"] }
```

and adds its own package groups below that line. Renovate runs as the hosted
[Mend Renovate app](https://github.com/apps/renovate) and reads the preset from `main` of this repository, so a
change here reaches every opted-in repository on the app's next run. Check a change before merging with

```shell
npx --package renovate -- renovate-config-validator --strict renovate-config.json5
```
