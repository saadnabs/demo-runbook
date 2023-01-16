# Web App user issues

If you are running into issues with the regularity of your web application users, there are different things you can do

## Troubleshooting

First step is to better understand the standard behaviour and dig into what the current metrics are showing
For this, the [following dashboard](https://se-demo.grafana.net/d/9ako2pfZz/web-app-observability-dashboard?orgId=1&refresh=5s) has already been setup to help you

Make sure you look at extended time ranges and check for any firing alerts

## Debugging

If you've been able to find more information about what is causing the issue, to dig deeper, it is recommended to [Explore](https://se-demo.grafana.net/explore?orgId=1&left=%7B%22datasource%22:%22prometheus%22,%22queries%22:%5B%7B%22refId%22:%22A%22,%22datasource%22:%7B%22type%22:%22prometheus%22,%22uid%22:%22prometheus%22%7D%7D%5D,%22range%22:%7B%22from%22:%22now-1h%22,%22to%22:%22now%22%7D%7D) the data and start looking for the logs related to the incident. If traces are available, you should also be able to dig deeper in to the traces to find the section of code that may be causing the issue.

## Tracking

Any such issues should have a [new incident](https://sedemo.grafana.net/a/grafana-incident-app/incidents) created allowing for tracking of the issue, resolution and next steps to mitigate this and stop it from happening in the future
