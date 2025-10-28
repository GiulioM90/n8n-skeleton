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

## 🌍 ngrok (for Telegram webhooks)
ngrok creates secure tunnels to expose your local n8n to the internet, required for Telegram webhooks that need HTTPS.

### Setup ngrok
```bash
# Download from https://ngrok.com/ and authenticate
ngrok config add-authtoken YOUR_TOKEN
```

### Start tunnel
```bash
ngrok http 5678
```

### Update .env with ngrok URL
```env
NGROK_URL=https://your-ngrok-url.ngrok.io
```

### Restart n8n
```bash
docker compose restart
```

**Note:** ngrok URL changes on restart (free plan). Use localhost for development, ngrok only for webhooks.