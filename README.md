# Ollama on fly.io for Byrdson Services

1. `fly launch --copy-config --no-deploy --org byrdson-services`
2. `git restore fly.toml`
3. `fly deploy --flycast --ha=false`
4. `fly machine run -e OLLAMA_HOST=http://ollama-byrdson.flycast --shell --command "ollama pull llama3.2" ollama/ollama`