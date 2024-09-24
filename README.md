# BLOG API
Esta é uma API de um Blog desenvolvida com Node.js, Express e MongoDB. A API permite criar, editar, deletar e procurar postagens deste blog. Os testes são escritos com Jest e a documentação da API é gerada com o Swagger.

### Índice
- Instalação
- Configuração
- Endpoints da API
- Testes
- Documentação Swagger
- Estrutura de pastas
- Tecnologia utilizada

### Instalação
1. Clone o repositório
`git clone https://github.com/fhamamura/blog.git`

2. Navegue até o diretório do projeto:
`cd blog`

3. Instale as dependências
`npm install`

4. Inicie o servidor
`npm start`

O servidor irá rodar em `https://localhost:3000`.

### Configuração
Crie um arquivo `.env` na raiz do projeto com as seguintes variáveis de ambiente:
```
PORT=3000
MONGO_URI="mongodb://localhost:27017/mongo"
```
- `PORT` : Define a porta em que o servidor será executado.

- `MONGO_URI` : String de conexão ao MongoDB.

### Endpoints da API
#### Listar todos os Posts
- GET `/posts`
#### Obter um Post por ID
- GET `/posts/:id`
#### Criar um Post
- POST `/posts`
  
	Body:
```
{
  "title": "Título do Post",
  "content": "Conteúdo do Post",
  "author": "Autor do Post"
}
```
