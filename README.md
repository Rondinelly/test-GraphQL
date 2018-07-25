# GraphQL

Atualmente, a maioria dos aplicativos tem a necessidade de buscar dados de um servidor no qual os dados são armazenados em um banco de dados. É responsabilidade da API fornecer uma interface para os dados armazenados que atenda às necessidades de um aplicativo.
Em suma, uma API define como um cliente pode carregar dados de um servidor.


## GraphQL é uma linguagem de consulta para APIs ?

GraphQL é um novo padrão de API que fornece uma alternativa mais eficiente e flexível ao REST.
GraphQL permite que o cliente possa especificar exatamente quais dados precisa de uma API. Em vez de vários pontos que retornam estruturas de dados fixas, um servidor GraphQL apenas expõe um único ponto e responde precisamente com os dados solicitados por um cliente.

## Rest

REST é uma maneira popular de buscar dados de um servidor. Quando o conceito REST foi desenvolvido, os aplicativos eram relativamente simples e o ritmo de desenvolvimento não estava exatamente onde está hoje. REST, portanto, foi um bom ajuste para muitas aplicações. No entanto, o panorama da API mudou radicalmente nos últimos anos.

## Problemas ?

- **Um aplicativo de conteúdo que precisa exibir os títulos de postagens de um usuário específico**

Com uma API REST, normalmente, se acessa os dados usando vários endpoint.
Esses podem ser  `/users/<id>`, por exemplo, o ponto para buscar os dados iniciais do usuário.
Em segundo lugar, é provável que haja um `/users/<id>/posts` terminal que retorne todas as postagens 
para um usuário. O terceiro endpoint será o `/users/<id>/followers`que retorna uma lista de seguidores por usuário.

Com REST, temos que fazer três solicitações para diferentes endpoints para buscar os dados necessários. Também estamos fazendo 
overfetching, já que os endpoints retornam informações adicionais desnecessárias.

No GraphQL, por outro lado, nós simplesmente enviamos uma única consulta para o servidor GraphQL que inclui os requisitos de dados concretos. Em seguida, o servidor responde com um objeto JSON em que esses requisitos são atendidos.

Usando GraphQL, o cliente pode especificar exatamente os dados necessários em uma consulta. A estrutura da resposta do servidor segue precisamente a estrutura aninhada definida na consulta.





