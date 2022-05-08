# Helm Chart Releaser Repo

## Development flow for Helm Charts

- helm create <chart-name>
- Edit Values.yaml
- Edit Chart.yaml
- Lint your chart 
`ct lint --charts ./<chart>`
- Test the installation of the chart
`ct install --charts ./<chart>`


## Chart Releaser CLI (cr)

## Chart Tester CLI (ct)