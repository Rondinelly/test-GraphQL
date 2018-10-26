# GraphQL

Atualmente, a maioria dos aplicativos tem a necessidade de buscar dados 
em um servidor, no qual são armazenados em um banco de dados. É 
responsabilidade da API fornecer uma interface de comunicação, 
para que os dados armazenados possam ser enviados ao aplicativo, que 
processa e devolve informações. Resumindo, uma API define como um 
cliente pode enviar e receber dados de um servidor.

## GraphQL é uma linguagem de consulta para APIs 

GraphQL é um novo padrão de API que fornece uma alternativa mais 
eficiente ao REST. GraphQL permite que o cliente especifique
exatamente quais dados lhe são necessários. Ao contrário de 
vários _endpoints_ que retornam estruturas de dados fixas, um
servidor GraphQL apenas expõe um único _endpoint_ e responde 
precisamente com os dados solicitados pela `query`.

Com uma API REST, normalmente, se acessam dados usando vários 
_endpoints_. Esses podem ser `/users/<id>`, por exemplo, o 
_endpoint_ para buscar os dados de determinado usuário. Mas, 
é provável que haja um `/users/<id>/posts` que retorne todas as
postagens de um usuário. Mais outro _endpoint_ 
`/users/<id>/followers` que retorna uma lista de seguidores por 
usuário. Com REST, temos que fazer três solicitações diferentes, 
com três _endpoints_ diferentes, para buscar os dados necessários. 
Fazendo _overfetching_, já que os _endpoints_ retornam informações 
adicionais desnecessárias. Em GraphQL, por outro lado, é enviado uma
única consulta, na qual o servidor que inclui os requisitos com dados 
concretos. Em seguida, o servidor GraphQL responde um objeto JSON com 
esses requisitos atendidos. O cliente pode especificar exatamente os 
dados necessários em uma consulta. A estrutura da resposta do servidor 
segue precisamente a estrutura aninhada definida na consulta.

## Queries 

É o processo de buscar resultados do servidor GraphQL. 

## Mutations 

É o processo de escrever operações no servidor GraphQL. 
Permitiria ao usuário modificar os dados do lado do servidor.
Semelhante a realizar solicitações `POST` no REST, qualquer 
operação escrita tem que ser enviada através de uma `mutation`.

## Introspection

Torna possível declarar um esquema JSON de forma compatível a 
diferentes implementações, independente da linguagem. É projetada 
para ser coletada via execução



