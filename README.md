# Helm Chart Releaser Repo
[![Artifact Hub](https://img.shields.io/endpoint?url=https://artifacthub.io/badge/repository/patricklaabs)](https://artifacthub.io/packages/search?repo=patricklaabs)

## Development flow for Helm Charts

- create a new feature-branch
- helm create <chart-name>
- Edit Values.yaml
- Edit Chart.yaml
- Lint your chart 
`ct lint --charts ./<chart>`
- Test the installation of the chart
`ct install --charts ./<chart>`
- push and create a pr

## Chart Releaser CLI (cr)

- cr package --config config.yaml ./charts/*
- cr upload --config config.yaml --skip-existing
- cr index --config config.yaml