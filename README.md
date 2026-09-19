# Conect Obra — Site final

## Publicação online

O projeto já possui configuração `render.yaml` para hospedagem de uma aplicação Node.js.

### Opção de publicação
1. Crie uma conta em um serviço de hospedagem compatível com Node.js.
2. Coloque este projeto em um repositório Git.
3. Crie um Web Service apontando para o repositório.
4. O comando de build é `npm install`.
5. O comando de inicialização é `npm start`.
6. O health check é `/api/health`.

### Importante
Esta versão usa `data/db.json` para persistência local. Em hospedagem com filesystem efêmero, os dados não devem ser tratados como banco de produção. Para o lançamento real do marketplace, migre usuários, obras, propostas, mensagens e avaliações para PostgreSQL/Supabase ou outro banco persistente.

Também será necessário configurar domínio/HTTPS, autenticação segura, recuperação de senha, armazenamento de fotos/documentos e adequação à LGPD antes de uma operação comercial em escala.

## Execução local
`npm install`
`npm start`

Depois abra `http://localhost:3000`.
