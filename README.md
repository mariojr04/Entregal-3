# API de Operações Matemáticas
Este projeto é uma API simples construída com Node.js e Express, que permite realizar operações matemáticas básicas: soma, subtração, multiplicação e divisão.

## Requisitos
Antes de começar, você precisa ter instalado:
- Node.js (que já inclui o NPM).
  
## Como usar este projeto
### 1. Clonar o repositório 
Primeiro, você precisa clonar este repositório para sua máquina local. Abra o terminal e execute:

````bash
git clone https://github.com/seu-usuario/nome-do-repositorio.git
````
Substitua  `` seu-usuario ``  e `` nome-do-repositorio `` pelo seu nome de usuário e nome do repositório.

### 2. Navegar até a pasta do projeto
No terminal, navegue até a pasta do projeto:

````bash
cd nome-do-repositorio
````
### 3. Instalar dependências
Instale as dependências necessárias usando o NPM. Execute o seguinte comando:

````bash
npm install express body-parser
````
### 4. Executar o servidor
Para iniciar o servidor, execute:

````bash
node app.js
````
Você verá a mensagem: `` App de Exemplo escutando na porta http://localhost:3001/. ``

### 5. Testar as operações matemáticas
Agora você pode testar as operações matemáticas usando uma ferramenta chamada Postman. O Postman permite enviar requisições HTTP para o seu servidor.

#### 5.1. Instalar o Postman
Se você ainda não tem o Postman, baixe e instale a partir do site oficial: Postman.

#### 5.2. Enviar requisições
1. Abrir o Postman.
2. Criar uma nova requisição.
- Selecione `` POST ``.
- Na barra de endereço, insira ``http://localhost:3001/somar`` para somar, ou mude para ``/subtrair``, ``/multiplicar`` ou ``/dividir`` conforme necessário.
3. Na aba "Body", selecione ``raw`` e escolha ``JSON``.
4. Envie o seguinte JSON no corpo da requisição:
```` json

{
  "a": 5,
  "b": 10
}
````
Clique em ``Send``.
### 6. Resultados
Após enviar a requisição, você verá a resposta do servidor:


- Para a soma: "O resultado da soma de 5 e 10 é 15."
- Para a subtração: "O resultado da subtração de 5 e 10 é -5."
- Para a multiplicação: "O resultado da multiplicação de 5 e 10 é 50."
- Para a divisão: "O resultado da divisão de 5 e 10 é 0.5."
  
### 7. Mensagens de erro
Se você não enviar números válidos, o servidor responderá com uma mensagem de erro informando que é necessário fornecer números válidos.

## Estrutura do Código
- Express: Um framework para Node.js que facilita a criação de servidores.
- Body-Parser: Uma biblioteca que ajuda a ler os dados enviados nas requisições.
### Funções principais
- ``soma(a, b)``: Função que realiza a soma de dois números.
- Rotas para operações:`` /somar``, ``/subtrair``, ``/multiplicar``, ``/dividir``.
## Conclusão
Agora você tem uma API simples que pode realizar operações matemáticas básicas. Sinta-se à vontade para modificar e expandir o código!
