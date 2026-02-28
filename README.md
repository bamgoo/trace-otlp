# trace-otlp

bamgoo otlp trace driver (HTTP endpoint).

```toml
[trace.otlp]
driver = "otlp"
fields = { trace_id = "bamgoo.trace_id", span_id = "bamgoo.span_id" }
[trace.otlp.setting]
endpoint = "http://127.0.0.1:4318/v1/traces"
timeout = "5s"
service = "my-service"
headers = { "Authorization" = "Bearer token" }
```

`fields` is configured on `[trace.otlp]` (not under `setting`).
