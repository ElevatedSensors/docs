# Elevated Sensors Documentation

[![Netlify Status](https://api.netlify.com/api/v1/badges/b9fb3e12-fc9b-47d5-a313-872e118406f9/deploy-status)](https://docs.elevatedsensors.com)
[![License: MIT](https://img.shields.io/badge/License-MIT-blue.svg)](LICENSE)
[![Last Commit](https://img.shields.io/github/last-commit/ElevatedSensors/docs/main)](https://github.com/ElevatedSensors/docs/commits/main)
[![GitHub issues](https://img.shields.io/github/issues/ElevatedSensors/docs.svg)](https://github.com/ElevatedSensors/docs/issues)

**Live Documentation:** [https://docs.elevatedsensors.com](https://docs.elevatedsensors.com)

This repository contains the source files for the Elevated Sensors documentation site, built with [Zensical](https://zensical.org/). It includes product manuals, integration guides, firmware manifests, and automation examples.

## Contributing

Contributions are welcome!  
- Add or update Markdown files in the `docs/` folder.
- Assets (images, PDFs, CSS) go under `docs/assets/`.
- Follow existing folder structure: `products/`, `integrations/`, `guides/`.
- Open a pull request and describe your changes.

## Folder Structure

```
docs/
├─ index.md                 # Home page
├─ products/                # Product-specific pages
├─ integrations/            # Integration-specific pages
├─ guides/                  # Automation examples, general guides
└─ assets/                  # Images, CSS, PDFs
```

## Setup/Local Preview

1. Fork the repository and clone it
   ```bash
   git clone https://github.com/<your-username>/docs.git
   cd docs
   ```
1. Install Zensical
   ```bash
   python3 -m venv .venv
   source .venv/bin/activate  # On Windows: .venv/Scripts/activate
   pip install zensical
   ```
1. Run the preview server
   ```bash
   zensical serve
   ```
1. Access the docs at `http://localhost:8000`
