# MW LLM Proxy

Setup a proxy with litellm to use the mittwald AI hosting in your IDE.

1. Copy `.env.example`
   ```
   cp .env.example .env
   ```
2. Adjust `.env` and set your key in `MITTWALD_LLM_HOSTING_KEY`
3. Start the container
   ```
   docker compose up
   # or
   docker compose up --detached
   ```

## Setup in PhpStorm

![PhpStorm Settings to setup the Proxy as an AI provider](./img/ai-assistant-settings.png)

* Open Settings. Go to Tools › AI Assistant › Models
* Choose OpenAI API as a provider
* Set URL to `http://localhost:4000/v1`
