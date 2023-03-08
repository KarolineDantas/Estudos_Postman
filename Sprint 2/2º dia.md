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
