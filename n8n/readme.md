# n8n notebook
n8n Docs: https://docs.n8n.io

### Installed using docker
``` shell
docker run -d --name n8n -p 5678:5678 -p 5679:5679 -v "./volume/home/node/.n8n:/home/node/.n8n" --restart=on-failure --env GENERIC_TIMEZONE="Asia/Hong_Kong" --env TZ="Asia/Hong_Kong" --env N8N_BLOCK_FILE_ACCESS_TO_N8N_FILES=false --env N8N_RUNNERS_ENABLED=true --env N8N_ENFORCE_SETTINGS_FILE_PERMISSIONS=true docker.n8n.io/n8nio/n8n:1.93.0
```

### Installed using docker compose (n8n + postgresql)
``` shell
// cwd is ./n8n
docker compose -p workflow --env-file ./.env -f ./docker-compose.yml up -d --build --remove-orphans
```
