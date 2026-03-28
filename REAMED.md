O Ollama está acessível mas não tem nenhum modelo instalado! Precisa baixar o llama3 e o mistral:

docker exec ollama ollama pull llama3
docker exec ollama ollama pull mistral


docker exec -it openclaw openclaw dashboard --no-open  
docker exec -it openclaw openclaw devices list   
docker exec -it openclaw openclaw devices approve 693950bb-f95a-4392-b341-794b7544da83

docker exec -it openclaw openclaw dashboard --no-open

docker exec -it openclaw openclaw devices list
docker exec -it openclaw openclaw devices approve --latest


#Enabled Whatsapp
docker exec -it openclaw openclaw plugins install @openclaw/whatsapp
docker exec -it openclaw openclaw channels login --channel whatsapp --verbose
docker compose restart openclaw

# image
docker exec -it ollama ollama pull qwen2.5-coder:14b
