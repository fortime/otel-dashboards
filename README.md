# otel-dashboards
Grafana dashboards with opentelemetry data from influxdb.

## Otel Trace Log
Currently because I can't set `frame.meta.preferredVisualisationType` to `'trace'`. Trace won't be shown. This dashboard can only show in a patched grafana. Remove `&& props.dataFrames[0]?.meta?.preferredVisualisationType === 'trace' ` in this [line](https://github.com/grafana/grafana/blob/main/public/app/features/explore/TraceView/TraceView.tsx#L146).
