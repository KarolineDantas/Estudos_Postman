## Introdução ao HTTP

### O que é API?

API (Aplication Programmin Interface ou Interface de Programação de Aplicações) refere-se a serviços que são uma forma de integrar sistemas, possibilitanto benefícios como a segurança dos dados, facilidade no intercâmbio entre informações de diferentes linguagens de programação e a monetização de acessos.

### Vantagens

<img width="584" alt="image" src="https://user-images.githubusercontent.com/107884724/223729785-bd344300-77af-43a8-8daa-04a11a447461.png">

Em outras palavras:

	• Facilita a comunicação entre diferentes partes de um sistema;
	
	• Agiliza o desenvolvimento (evita escrever muitos códigos);
	
	• O código tem maior qualidade;
	
	• O código possui maior segurança;

	• Em exemplos mais práticos, um cliente chega em um restaurante e acessa o cardápio. O garçom anota o pedido e passa para a chefe de cozinha. O garçom seria o API, a chefe seria o back-end e onde o cliente está é o front-end.

## Introdução ao HTTP
O HTTP é um protocolo usado para obter recursos, como por exemplo documentos HTML que vemos e utilizamos diariamente na web. Serve também para mediar a comunicação entre APIs.

<img width="640" alt="image" src="https://user-images.githubusercontent.com/107884724/223733176-3026aac2-0d42-4380-992a-04db512194e9.png">
O que é API?
API significa Application Programming Interface (Interface de Programação de Aplicação). Podemos dizer que a API é a “ponte” que conecta sistemas. Com ela, é possível que dois programas “conversem” entre si e integrem suas funcionalidades. Exemplo você acessa o aplicativo da Decolar para pesquisar uma passagem aérea, o aplicativo mostra as opções de diversas Cia. Essa informação é possível através das API que as cias aéreas disponibiliza para o aplicativo. Então a Decolar, consome APIs da Gol, Tam, etc. Para conseguir disponibilizar essas informações. Nesse caso podemos dizer que a Decolar é o cliente e Cia aérea é o servidor. Como os código não precisa ser reescrito do zero isso acaba trazendo muitas vantagens. Quais as vantagens de usar API? • Redução de custos • Segurança • Melhoria na comunicação • Inovação
Agora que entendemos o que é API, vamos entender o que é APIRest
O que é API Rest? REST significa Transferência Representacional de Estado.
O que isso quer dizer? É um estilo de arquitetura, que define padrões que facilita a comunicação entre sistemas web e usa o protocolo HTTP, é baseado em um contrato. Essa representação de estado pode estar no formato JSON, XML ou HTML. Hoje o mais usado é o Json.
Agora a Karol vai falar sobre o protocolo HTTP.Validações em requisições HTTP
O HTTP é um protocolo que serve como base na comunicação que existe em toda a
Internet. Além disso, o HTTP serve também para intermediar a comunicação com
APIs.
O fluxo de comunicação é realizado a partir do cliente, que envia uma requisição ao
servidor usando o protocolo HTTP. Logo depois, o servidor interpreta, processa e
devolve a resposta.
Qual a estrutura de uma requisição? Bom, ela é formada pelos seguintes elementos:
• O método, que explica o tipo de requisição. Os mais utilizados são:
o GET : utilizado para a leitura de dados
o POST : criação de novos dados
o PUT: atualização de dados
o DELETE : exclusão de dados
• A URL, que é o caminho do recurso (endpoint);
• A versão do protocolo HTTP;
• Cabeçalho, que contém informações sobre a requisição;
• Um corpo de dados.
Já a resposta do servidor possui elementos:
• A versão do protocolo HTTP;
• Status de resposta;
• E o corpo (opcional)
Além disso, na resposta do servidor podemos obter algumas informações muito
importantes, como o status code. O status code serve para entender como o servidor
lidou com a requisição feita pelo cliente.
O status code é composto por 3 dígitos. Se começar com:
• 1xx - Indica que o servidor ainda está processando a requisição de alguma
forma.
• 2xx - A requisição foi completamente recebida e o servidor entregou ao cliente
o recurso esperado.
• 3xx - A requisição foi recebida, mas o servidor precisou realizar algum tipo de
redirecionamento.
• 4xx - Códigos nesse range geralmente indicam um problema nas informações
enviadas pelo cliente.
• 5xx - Os códigos nesse intervalo correspondem a erros relacionados ao
servidor.O que validar em uma API?
Testes Técnicos (de acordo com o que foi especificado na Swagger da API)
• Validar o status code retornado
• Validar o header de retorno;
• Validar o body do response;
• Validar o tempo de resposta;
Testes funcionais
• Validar como sua API se comporta quando o serviço está fora;
• Validar o resultado obtido X o resultado esperando, sempre se baseando na
Swagger da API;
• Validar o comportamento da API quando enviado um JSON com uma estrutura
incorreta.
Agora o Vinicius vai falar um pouco sobre os objetos Json.
O que são objetos JSON (sua aplicação em APIs
REST)
JSON é um acrônimo para JavaScript Object Notation, e como o nome sugere, é uma
forma de notação de objetos JavaScript, de uma forma que esses objetos podem ser
representados em diversas linguagens. É um formato leve para intercâmbio de dados.
Mesmo sendo baseado em JavaScript, o JSON não é uma linguagem de
programação, é uma notação para transferência de dados que segue um padrão. Ele
sempre é composto por texto e não possui comentários ou funções dentro de sua
composição.
O padrão dos dados usados dentro de um JSON é estruturado por meio de uma
coleção de pares com nome e valor ou uma lista ordenada de valores.
Esses pares sempre são compostos por uma chave e um valor, onde a chave é a
identificação do conteúdo e os valores são os conteúdos. Os valores podem conter
os seguintes tipos de dados: string, array, object, number, boolean ou null.
A formatação dos arquivos JSON sempre é feita por alguns caracteres específicos,
são eles:
Chaves {} : para delimitar os objetos e também para iniciar e encerrar o JSON.
Colchetes [] : para delimitar um Array.
Dois pontos : : para separar a chave de seu valor.Vírgula , : para indicar a separação entre os elementos.
### Verbos HTTP e Status Code

## Arquitetura de microsserviços X monolítico

|Microserviços|
|--|
|Cada serviço é desenvolvido em torno de um conjunto de regras de negócio específico, e é implementado de forma independente. Se pudéssemos resumir a arquitetura de microsserviços em uma palavra, seria especialização. Como cada serviço tem uma implantação diferente, a subida de uma nova versão não atrapalha a disponibilidade dos demais.|
|**Vantagens**:
• É mais fácil evoluir o sistema e fazer a  manutenção;
• Possui maior escalabilidade;
• Redução de custos;
• Mais flexibilidade
**Desvantagens**:
• Mais complexo.
|

		
|Monolítica|
|--|
|Todas as funções do negócio estão implementadas em um único processo. Os diversos módulos do sistema são executados em uma mesma máquina, compartilhando recursos de processamento, memória, bancos de dados e arquivos.|
|**Vantagens**:
• Mais fácil de entender.
**Desvantagens**:
• • Dificuldade na escalabilidade;
• Alta dependência de componentes de código;
• Se você mexer em um lugar pode gerar problemas em outro, justamente por estar tudo interligado;
• Falta de flexibilidade 
|


## Rest e Restful

**Rest** 
	• Determina algumas obrigações nas transferências de dados do API;
	
	• A API geralmente utiliza o protocolo HTTP para a transferência de dados;
	
	• Dados no Rest é chamado de Resources, que basicamente pode ser uma entidade ou objeto.
	

**Necessidades para ser Restful**
Para ser Restful é necessário aplicar os padrões Rest. Mas quais são esses padrões?

1. Cliente_server
- Separação do cliente e do armazenamento de dados (servidor), dessa forma poderemos ter uma portabilidade do sistema, usando o React para WEB e React Native para o celular, por exemplo;
		
- Ou seja, mudanças feitas pelo usuário na aplicação em seu dispositivo não devem afetar o servidor e sua estrutura de dados. De mesmo modo, alterações feitas pelos desenvolvedores nos bancos de dados da aplicação não devem instantaneamente impactar o dispositivo do usuário.

2. Stateless
- Cada requisição que o cliente faz para o servidor deverá conter todas as informações necessárias para o servidor entender e responder (response) a requisição (request);
		
- É como em um restaurante, o garçom anota os pedidos e precisa saber qual mesa pediu o quê;
		
- Em uma REST API, cada solicitação contém todos os dados necessários para que seja atendida, não dependendo de informações já armazenadas em outras sessões.
		
	
3. Cache
- As respostas para uma requisição deverão ser explicitas ao dizer se aquela requisição pode ou não ser cacheada pelo cliente;
		
- Uma API REST deve ser desenvolvida de modo que consiga armazenar dados em cache. Quando uma informação fica armazenada em cache, as solicitações e respostas entre cliente e servidor são otimizadas.
		
4. Layered System
- O cliente acessa a um endpoint sem precisar saber da complexidade, de qual passos estão sendo necessários para o servidor responder a requisição, ou quais outras camadas o servidor lida para que a requisição seja respondida.
