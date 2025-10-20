# 🧩 n8n Docker Quickstart

Basic commands to run and manage n8n using Docker Compose.


## 🚀 Start the container
- docker compose up -d

## 🛑 Stop the container
- docker compose stop

## 🔁 Restart the container
- docker compose start

## 📜 View logs
- docker compose logs -f

## ❌ Remove container and volume (reset)
- docker compose down -v

## 🧼 Update to the latest version
- docker compose pull && docker compose up -d

## Access on ui 
- http://localhost:Port