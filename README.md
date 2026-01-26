## 👋 Welcome to clipcascade 🚀

Universal clipboard manager with sync across devices

## 📋 Description

Universal clipboard manager with sync across devices

## 🚀 Services

- **app**: sathvikrao/clipcascade:latest

## 📦 Installation

### Option 1: Quick Install
```bash
curl -q -LSsf "https://raw.githubusercontent.com/composemgr/clipcascade/main/docker-compose.yaml" -o compose.yml
```

### Option 2: Git Clone
```bash
git clone "https://github.com/composemgr/clipcascade" ~/.local/srv/docker/clipcascade
cd ~/.local/srv/docker/clipcascade
docker compose up -d
```

### Option 3: Using composemgr
```bash
composemgr install clipcascade
```

## 🔧 Configuration

### Environment Variables

```shell
TZ=America/New_York
APP_USER_NAME=administrator
APP_USER_PASS=changeme_user_password
```

See `docker-compose.yaml` for complete list of configurable options.

## 🌐 Access

- **Web Interface**: http://172.17.0.1:59063

## 📂 Volumes

- `./rootfs/data/clipcascade` - Data storage

## 🔐 Security

- Change all default passwords before deploying to production
- Use strong secrets for all authentication tokens
- Configure HTTPS using a reverse proxy (nginx, traefik, caddy)
- Regularly update Docker images for security patches
- Backup your data regularly

## 🔍 Logging

```shell
docker compose logs -f app
```

## 🛠️ Management

```bash
# Start services
docker compose up -d

# Stop services
docker compose down

# Update to latest images
docker compose pull && docker compose up -d

# View logs
docker compose logs -f

# Restart services
docker compose restart
```

## 📋 Requirements

- Docker Engine 20.10+
- Docker Compose V2+

## 🤝 Author

🤖 casjay: [Github](https://github.com/casjay) 🤖  
🦄 composemgr: [Github](https://github.com/composemgr) 🦄
