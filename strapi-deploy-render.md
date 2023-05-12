# Strapi deploy render

## Passo 1

Ir no dashboard do render,selecionar New + e depois Web Service

## Passo 2

Selecione o repositorio do github que ta o projeto strapi

## Passo 3

Nos campos:

Name: escolha um nome pro projeto
Region: pode deixar a padrao
Branch: main
Root directory: em branco
Runtime: Node
Build comand: yarn && NODE_ENV=production yarn build
Start comand: yarn start

# Passo 4

Clickar no botāo Advanced

# Passo 5

Clickar no botāo Add secret file, em name colocar .env e no content colocar o conteudo do .env do projeto

# Passo 6

Clickar em create web service

# Passo 7

Após terminar o build, vá em settings no projeto

# Passo 8

Procure por custom domains e aperte em Add custom domain

# Passo 9

Adicione api.NOME_DO_SITE.com.br, vai aparecer um link que vc vai usar no passo 11

# Passo 10

Vai la no registro.br e vai nas configuracoes de DNS

# Passo 11

Criar nova entrada do tipo CNAME com nome api e valor sendo o que apareceu no dashboard anteriormente

# Passo 12

Clickar em new + > static site e selecionar o mesmo repositorio

# Passo 13

Nos campos:

Name: escolha um nome pro projeto
Branch: main
Root directory: em branco
Build comand: yarn && NODE_ENV=production yarn build
Publish directory: ./dist/build

# Passo 14

Clickar no botāo Advanced

# Passo 15

Clickar no botāo Add secret file, em name colocar .env e no content colocar o conteudo do .env do projeto