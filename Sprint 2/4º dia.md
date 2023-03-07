

API - conceitos

O que validar em uma API?

	• Validar o status retornado;
	
	• Validar o header de retorno;
	
	• Validar o body do response;
	
	• Validar como sua API se comporta quando o serviço está fora;
	
	• Validar o comportamento da API quando enviado um JSON/XML com uma estrutura incorreta;
	
	• Validar o retorno com base nos requisitos definidos para cada tipo de dado enviado em sua API.


Existem alguns erros mais comuns para os quais você também pode se atentar ao testar sua API, veja quais são:

	• A API pode não atender a estrutura de dados enviada;
	
	• Erros de segurança;
	
	• Problemas de Multi-threading;
	
	• Não implementação de retornos para erros em determinados cenários.

Dinâmica de como funciona uma API

APIs podem ser implementadas de diversas formas, umas delas é seguindo uma arquitetura chamada Rest (Transferência Representacional de Estado).



Passo a passo de como funciona:
	1. A Lojinha API vai armazenar as regras de negócio da Lojinha e será responsável pelos recursos que a lojinha possui, como Produtos, Vendas, etc,;
	
	2. Se eu quiser testar se a Lojinha é capaz de permitir que alguém com os dados do Kleber consiga fazer login e ver os produtos dele, preciso ser o App e conversar com a API Rest da Lojinha enviando os dados do Kleber e esperar que ela me dê um Token se eu informar os dados do Kleber corretamente;
	
	3. Quando o App quer requisitar algo à API Rest da Lojinha, ele envia uma Requisição;
	
	4. A API Rest da Lojinha, por sua vez processa a informação da Requisição, então devolve uma Resposta. Ambas tem Cabeçalho e Corpo, mas apenas a Requisição tem URI e Método;

		
O que significa API em palavras simples
			
Uma API é um meio pelo qual dois sistemas possam se comunicar.
	
Em exemplos mais práticos:
			
	• Quando você pluga o seu notebook em uma tomada, podemos dizer que a tomada é uma API que fornece energia para o seu equipamento ou
	
	• quando você atravessa uma ponte de carro, então podemos dizer que a ponte é uma API que permite conectar duas rodovias e ainda
	
	• quando você coloca uma nova lâmpada em sua luminária, a base da luminária é uma API para a sua lâmpada.
		
Por que existem as APIs?
	
Quando voltamos ao início da era PC (com o surgimento do 286, 386 etc) – e até mesmo antes disto – quando se queria imprimir um documento por um software, certamente o fabricante do software não fornecia uma impressora para o usuário, mas 

aquele software podia chamar uma API da impressora e então imprimir o documento. O mesmo vale para por exemplo exibir algum caractere no monitor. A rotina que exibe um caractere no monitor do usuário é uma API de baixo nível chamada para exibir aquele caractere.

O motivo pelo qual as APIs estão cada vez mais evidência é o fato de que as APIs deixaram de ser apenas um modelo arquitetural de software, mas passou a ser um pre-requisito de negócios, pois através delas é possível criar uma série de novos modelos de negócios. É o que estamos chamando de API Economy ou Economia das API.


Como uma API Rest é testada?

Massa de dados para teste de API
A massa de dados para o teste de API se dá a partir de uma estrutura de dados que será enviada para a API, essa estrutura pode ser um arquivo JSON ou XML contendo os parâmetros da sua API.

Com a estrutura de dados pronta basta informar os dados no BODY da sua requisição para realizar a chamada da API e então validar os retornos apresentados.

De <https://blog.cedrotech.com/como-testar-uma-api-de-forma-amigavel> 

	5. Para que o App consiga se comunicar com a API Rest da Lojinha, é necessário saber qual é o endereço de onde ela está localizada e também qual recurso queremos utilizar. Já sabemos essas informações. O endereço é http://api.lojinha.com e o recurso é o login, logo, acabamos de ter nossa URI: http://api.lojinha.com/login. Assim, preencheremos ela naquela caixa da Requisição da página anterior;
	
	6. Além da URI também precisamos do Método, ele serve para dizer à API Rest qual ação ela precisa executar, por exemplo, "Registrar". 
	Há 4 métodos muito conhecidos em Rest:  
	
		○ Buscar, representado por GET; 
		○ Registrar, representado por POST; 
		○ Alterar, representado por PUT; 
		○ Remover, representado por DELETE. 
	
	Logo, se nosso teste envolve registrar o Login, o método que colocaremos na caixa de Requisição é o POST.
	
	7. Por fim, antes de enviarmos a Requisição para a API Rest da Lojinha, teremos que informar os dados do Kleber. Para isso, preciso descrever os dados dele no formato JSON: 
	{ " usuarioLogin" : "klebinho" , 
	" usuarioSenha" : 123456 
	} 
	No formato JSON temos chaves representando um objeto. Um objeto tem atributos, no caso, usuarioLogin e usuarioSenha. Atributos tem valores, "klebinho" e 123456.

Como estamos enviando um JSON no corpo, precisamos informar isso no cabeçalho, usando um Content-Type com o valor "application/json". O JSON fica no corpo da Requisição. Nesse momento, nossa Requisição está assim:

Agora ela já pode ser enviada! Ao fazer isso, a API Rest da Lojinha recebe, converte e extrai os dados do corpo da Requisição e pesquisa no banco de dados se existe um usuário klebinho com senha 123456, se sim, ela devolve uma Resposta que possui um Cabeçalho e um Corpo. 

No cabeçalho, um código chamado Status Code, que é uma lista de números que descrevem a natureza da Resposta. O 201 significa "Criado" , no caso, o registro de login do Kleber. 

No corpo, veio o Token do Kleber. O Token serve para lembrar a API Rest da Lojinha quem é que a está chamando. Logo, guarde bem o Token, caso contrário nunca verá os produtos que pertencem ao Kleber!
{ 
"token" : "761b69db-ace4-49cd-84cb"
 }
Teste encerrado, deu certo!

Pontos importantes
Antes de testar uma API, pergunte-se:
• Qual é o propósito da API?
• Quem é o público-alvo?
• Quais problemas fazem parte dos testes?
• Qual é o resultado desejado?
• Quais são os recursos e as funções da API?
• Qual é o fluxo de trabalho da aplicação?
• Quais integrações a API aceita?
• Quais são as prioridades dos testes?
Também configure o ambiente dos testes, escolha as ferramentas de teste e o tipo de teste que irá aplicar.

Pode-se utilizar os testes:
• Teste funcional: testa diferentes funções na base do código. Os testes representam situações específicas para garantir que as funções da API funcionem dentro dos parâmetros planejados e esperados.
• Teste de confiabilidade: serve para confirmar que a API opera sem falhas durante um período específico num ambiente específico.
• Teste de carga: monitora o desempenho da API em condições normais e de pico.
• Teste de segurança: verifica se a API é segura contra ameaças externas. Os testes incluem 

metodologias de criptografia, controle de acesso à API, gerenciamento de direitos do usuário e validação da autorização.
• Teste da IU: envolve testar a interface de usuário da API. Seu foco é a interface vinculada à API, e não a própria API. Os testes de IU podem dar uma visão geral da integridade e da usabilidade do aplicativo no front-end e no back-end.
• Teste negativo: mostra o que acontece quando o aplicativo recebe uma entrada inválida ou não intencional. Assim, você descobre o que corta o sistema e, então, desenvolve respostas mais apropriadas. Por exemplo: adicionar uma letra num campo de números deve disparar aviso e não causar falha no aplicativo. 
• Teste de validação: serve para confirmar que a API foi desenvolvida corretamente e que tudo funciona.

De <https://www.lucidchart.com/blog/pt/teste-de-api-guia-completo> 

Teste manual x automatizado
O teste manual tem uma atenção mais focada no processo dos testes. Criar e executar manualmente os próprios testes dá a você um controle mais sutil sobre o processo. Além disso, há menos riscos de os testes gerarem falsos negativos, o que pode criar muito trabalho extra para validar os erros relatados como verdadeiros ou não.
Os seguintes tipos de testes podem ser manuais:
	• Testes exploratórios
	• Testes de usabilidade



• Testes de IU
• Testes ad hoc
É recomendável usar os testes manuais para observar pequenas mudanças. Até a menor alteração exige escrever um novo código para executar um teste automatizado, o que pode demorar mais do que fazer um breve teste manual. 


Por que usar o teste automatizado?
A maior vantagem na automação dos testes de API é fazer mais testes em menos tempo. Ela aumenta a produtividade e deixa os testes mais eficientes. Testes mais rápidos levam a correções mais rápidas e ao lançamento mais rápido dos produtos.
Os seguintes tipos de testes podem ser automatizados:
	• Testes funcionais
	• Teste de carregamento
	• Testes de desempenho
	• Testes de validação
	• Testes dinâmicos
	• Testes orientados por dados
	• Testes de erros
	• Testes em várias linguagens
	• Testes de regressão

Práticas recomendadas nos testes de API

	1. Documente tudo!
	2. Comece com APIs pequenas;
	3. Use a abordagem DRY.
	*A abordagem "não se repita" (DRY) serve para evitar a repetição de códigos. Se o código for comum a componentes e ações em várias APIs, inclua-o numa biblioteca que seja de fácil acesso a todos que precisarem dele.
![image](https://user-images.githubusercontent.com/107884724/223537626-47c6a536-81ac-4c0a-a5fc-1d604cd5790d.png)
