# LLM-Ink

Infrastructure complète pour déployer un serveur LLM local (CPU/GPU) avec [llama.cpp](https://github.com/ggerganov/llama.cpp), Docker, et API HTTP (port 5000).

## 🔧 Stack utilisée

- 🐋 Docker / Docker Compose
- 🧠 llama.cpp (compilé avec CMake)
- 📦 Mistral 7B Instruct GGUF (modèle par défaut)
- 🛡️ Volume monté sur `/mnt/volume-data` pour la persistance
- ⚙️ Portainer pour la gestion visuelle de Docker

## 🚀 Démarrage rapide

```bash
cd llm-server
docker compose up -d --build
```

## 📁 Arborescence

- `llm-server/` : Dockerfile + entrypoint.sh pour le serveur LLM
- `infra/` : Docker Compose pour Portainer
- `DOCUMENTATION.md` : historique technique du projet, étapes par étapes

## 🔐 Accès

- Portainer : http://<ip-vps>:9000
- API LLM : http://<ip-vps>:5000
