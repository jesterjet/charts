# How to publish new version

- Update version in Chart.yaml
- Update the necessary files in templates/ folder
- Generage the new package:

```bash
helm package jesterjet-mautic
```
- Update the `index.yaml` with:

```bash
helm repo index . --url https://charts.jesterjet.com/
```

- Commit and push the changes