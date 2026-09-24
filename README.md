# Qwen-Image 3.0 API (qwen-image-3.0 / qwenimage3.0) — api guide with published pricing

> **default $0.0206; 1K $0.0206; 2K $0.0206** — flat per-unit billing through the OpenAI-compatible APIMart gateway, $1 minimum top-up.

**[Live pricing](https://apimart.ai/pricing)** · **[Get an API key](https://apimart.ai/keys)**

Everything here refers to **qwen-image-3.0** — also written **qwenimage3.0** or **qwen image 3.0**.

## Pricing (observed, snapshot 2026-09-24)

| Tier | Price |
| --- | --- |
| `default` | $0.0206 |
| `1K` | $0.0206 |
| `2K` | $0.0206 |

## Cost at scale

| Volume | Cost |
| --- | --- |
| 100 | $2.0571 |
| 1,000 | $20.5712 |

## How to call it

```bash
curl --request POST --url https://api.apimart.ai/v1/images/generations \
  --header "Authorization: Bearer $APIMART_API_KEY" --header 'Content-Type: application/json' \
  --data '{"model":"qwen-image-3.0","prompt":"a modern cliffside villa at dusk","size":"16:9","n":1}'
```

Submit, keep the `task_id`, poll `GET /v1/tasks/{id}` until `completed`; the response carries the URL and the exact amount charged.

## Disclosure

Documents access through APIMart, a third-party API gateway; not affiliated with the model vendor.
