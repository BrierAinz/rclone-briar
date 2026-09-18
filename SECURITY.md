# Security

This repository is public documentation for a personal rclone configuration. It must never contain operational credentials or private backup metadata.

## Sensitive material that must stay out of Git

- `rclone.conf` or equivalent configuration exports
- OAuth client secrets, access tokens, refresh tokens, or token caches
- Private remote names when they reveal internal structure
- Personal file listings, backup manifests, or local filesystem paths
- Private keys or environment files

The repository `.gitignore` blocks common forms of these files, but ignore rules are a safeguard, not a substitute for review.

## If a credential is exposed

1. Treat it as compromised even if the commit is later deleted.
2. Revoke or rotate the affected OAuth/token material at the provider.
3. Remove the secret from the current tree and, when necessary, rewrite repository history.
4. Verify that no backup manifest or personal file listing was exposed alongside it.

Do not post active credentials in an issue, pull request, screenshot, or log.

## Scope

There is no network service or shared application hosted by this repository. Security reports are mainly relevant to accidental credential/data exposure in the repository itself or to unsafe documentation that would cause credentials to be published.
