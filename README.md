bash
cat > README.md << 'EOF'
# Laravel 11 Project

Este é um projeto Laravel 11 com configuração Docker para desenvolvimento.

## 📋 Pré-requisitos

- Docker
- Docker Compose

## 🚀 Passo a passo para rodar o projeto

### 1. Clone o projeto
```bash
git clone https://github.com/especializati/curso-laravel-11 laravel-11
cd laravel-11/
2. Crie o Arquivo .env
bash
cp .env.example .env
3. Configure as variáveis de ambiente
Atualize o arquivo .env com as seguintes configurações:

env
APP_NAME="Especializa Ti"
APP_URL=http://localhost:8989

DB_CONNECTION=mysql
DB_HOST=mysql
DB_PORT=3306
DB_DATABASE=nome_que_desejar_db
DB_USERNAME=nome_usuario
DB_PASSWORD=senha_aqui

CACHE_DRIVER=redis
QUEUE_CONNECTION=redis
SESSION_DRIVER=redis

REDIS_HOST=redis
REDIS_PASSWORD=null
REDIS_PORT=6379
4. Suba os containers do projeto
bash
docker-compose up -d
5. Acesse o container
bash
docker-compose exec app bash
6. Instale as dependências do projeto
bash
composer install
7. Gere a key do projeto Laravel
bash
php artisan key:generate
8. Acesse o projeto
Abra seu navegador e acesse: http://localhost:8989

🛠️ Tecnologias Utilizadas
Laravel 11

Docker

MySQL

Redis

Nginx

📝 Comandos Úteis
Para parar os containers:

bash
docker-compose down
Para ver os logs:

bash
docker-compose logs
Para recriar os containers:

bash
docker-compose up -d --force-recreate
🤝 Contribuição
Contribuições são sempre bem-vindas!

Desenvolvido com ❤️ usando Laravel 11
EOF

text

Agora para enviar para o GitHub:

```bash
# Adiciona o arquivo README.md
git add README.md

# Faz o commit
git commit -m "docs: create comprehensive README with setup instructions"

# Faz o push para o GitHub
git push origin main