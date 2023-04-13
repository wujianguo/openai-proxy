# openai-proxy
Proxy for OpenAI api using python flask, supports SSE streaming.

```python3 main.py```

``` shell
curl -N http://localhost:9000/v1/chat/completions \
  -H "Authorization: Bearer <your openai api key>" \
  -H "Content-Type: application/json" \
  -d '{"stream": true, "model": "gpt-3.5-turbo", "messages": [{"role": "user", "content": "What is the OpenAI mission?"}]}'
```
