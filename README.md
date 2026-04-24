# cydia.akemi.ai Archival Project

This project automatically archives [https://cydia.akemi.ai](https://cydia.akemi.ai) using the Wayback Machine and stores the results in GitHub Releases.

## How it works

A GitHub Action runs weekly (or manually) using a specialized `wayback` binary. It:
1. Downloads all available files for the website from the Wayback Machine.
2. Zips the content.
3. Creates a new GitHub Release with a date-based tag (e.g., `v2026.04.24`).
4. Uploads the archive to the release.

## Contents

- `wayback`: The archiver binary (Ubuntu x64).
- `.github/workflows/archive.yml`: The automation script.
