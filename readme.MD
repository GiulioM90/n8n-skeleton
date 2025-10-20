# 🧩 n8n Docker Quickstart

Basic commands to run and manage n8n using Docker Compose.

## 🚀 Start the container
```bash
docker compose up -d
```

## 🛑 Stop the container
```bash
docker compose stop
```

## 🔁 Restart the container
```bash
docker compose restart
```

## 📜 View logs
```bash
docker compose logs -f
```

## ❌ Remove container and volume (reset)
```bash
docker compose down -v
```

## 🧼 Update to latest version
```bash
docker compose pull && docker compose up -d
```

## 🌐 Access UI
Open in browser: http://localhost:5678