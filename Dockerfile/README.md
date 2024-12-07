# Trabalhando com Dockerfiles

## DESCRIÇÃO 

Inicialmente criei um Dockerfile apenas para entender como ele funciona em camadas e que cada comando gera uma camada extra utilizando o RUN. Também entendium pouco mais de como o Docker utiliza o cache para construir as imagens mais rapidamente, porém é necessário se atentar que alguns comandos são dependetes um do outro e que o cache pode ser um problema caso você necessite atualizar o versionamento de algum aplicativo. 
