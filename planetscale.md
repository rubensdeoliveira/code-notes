# Passo 1

Criar banco de dados no dashboard do planetscale

# Passo 2

Rodar `pscale login` para logar na conta desejada

# Passo 3 

Rodar `pscale database list` para verificar se os banco de dados disponiveis sāo os esperados

# Passo 4

Criar branch development no dashboard do planet scale da main, chame de development

# Passo 5

Rodar `pscale connect iope development`

# Passo 6

No .env adicionar: 

`DATABASE_URL="mysql://root@127.0.0.1:3306/NOME_DO_BANCO"`

> Trocar NOME_DO_BANCO pelo nome do seu banco

# Passo 7

Com planetscale invés de usar npx prisma migrate dev utilizar `npx prisma db push` pois a ideia do planetscale nāo é trabalhar com migrations e sim com branchs

# Passo 8

Agora pode ir no dashboard do planetscale e promover a branch development para main