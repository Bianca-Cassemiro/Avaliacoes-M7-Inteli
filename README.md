# Prova
Avaliações do Módulo 7

Clone este repositório e na raíz do projeto execute

```bash
docker compose -up -d
```
Com esse comando você irá baixar as imagens necessárias e o frontend estará rodando no localhost:3000 pronto para o uso.

Link do Dockerhub:
[https://hub.docker.com/repository/docker/bialimac/prova/general]

Backend
https://hub.docker.com/layers/bialimac/prova/backend/images/sha256-e2b78b0694f84cabc721f60d334e646b388cefd1a6676fd31d2f3c344a929644?context=repo

Frontend
https://hub.docker.com/layers/bialimac/prova/frontend/images/sha256-2566720b32e5f512d2ea44dee685a87aad6467f2bd3ca1f0c980cce801c1521b?context=repo

## Justificativas:
Para o docker file do backend a imagem que foi utilizada foi a do python:3.11 pois o backend foi feito utilizando python já para o frontend foi utilizada a imagem base do node:16.

Primeiro subi os containers separadamente e depois utilizei o docker compose para juntar as aplicações.

No frontend a porta 3000 é exposta e no backend a 8000.

Utilizando esta abordagem, qualquer pessoa consegue utilizar a aplicação sem se preocupar com arquivos do tipo "requirements.txt", onde deveria haver a instação de várias dependências específicas.
