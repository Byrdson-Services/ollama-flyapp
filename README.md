# Ollama on fly.io for Byrdson Services

1. `fly launch --copy-config --no-deploy --org byrdson-services`
2. `git restore fly.toml`
3. `fly deploy --flycast --ha=false`