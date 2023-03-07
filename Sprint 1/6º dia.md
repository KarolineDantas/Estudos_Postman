# Teste de Software: Introdução

### Para que servem os testes?
	• Para encontrar defeitos;
	• Verificar se o software está fazendo o que deveria;
	• Quanto mais cedo achar o erro melhor (e mais barato).

### O que deve ser testado?
	• Todos os casos de usos ou as funcionalidades mais críticas.

### Quando parar os testes?
	• Quando estiver confiante nos requisitos;
	• Quando os critérios de encerramentos forem atingidos;
	• Quando o custo para identificar os defeitos não compensa mais.

----------------------------------------------------------
# Apostila: Teste de Software
*Texto original [aqui](https://www.pjf.mg.gov.br/secretarias/sarh/edital/interno/selecao2015/arquivos/apostilas/modulo4_p.pdf).*

## 1. Teste de software
	• Serve para detectar erros e defeitos;
	• Mede a funcionalidade de um sistema.

### 1.1 Fundamentos do teste de software

**Objetivos do teste**	
	• Reduzir a probabilidade de incidência de erro;
	• Minimizar riscos aos negócios do cliente;
	• Atender as necessidades do cliente
	• Gerar um bom resultado > maior satisfação do cliente.

**Conceitos**
No resultado acima existe um erro, defeito e falha. Mas o que é cada um?
	• Erro = o programador colocou o símbolo * ao invés de +
	• Defeito = consequência do erro. O programa multiplica as entradas ao invés de somá-las 
	• Falha = consequência do defeito. O programa não conseguiu somar as duas entradas.


**Os defeitos podem ter as seguintes origens:**	
	• Prazo inadequado para atender às demandas, levando a não ter tempo suficiente para checar as atividades realizadas;
	• Tecnologia inadequada;
	• Falta de habilidade na equipe;
	• Não entender as necessidades do cliente;
	• Fator humano.
	
**Por que testar?**	
	• Diminuição de retrabalho;
	• Economiza tempo;
	• Encontrar falhas antes da produção  (o que é economicamente vantajoso);
	• Mais segurança aos clientes;
	• Melhora a qualidade e confiabilidade dos softwares;
	• Maior continuidade do serviço no negócio do cliente.

**Qual o custo?**
O custo da correção de um defeito tende a aumentar quanto mais tarde ele for encontrado.


**A psicologia do teste:**
Ter um grau de independência (pouca influência do autor) na hora de testar o software é uma opção eficiente. Existem níveis de independência:
	• A pessoa que escreveu o código irá testá-lo (baixo nível de independência);
	• Outras pessoas irão elaborar o teste (por exemplo, a equipe de desenvolvimento);
	• Teste elaborado por um grupo organizacional diferente (exemplo, equipe independente de testes);
	• Teste elaborado por diferentes organizações ou empresas (terceirizada, certificada, ou órgão externo).
	
É importante ter compreendido muito bem os objetivos do teste, para assim buscar os erros. É importante também saber comunicar de forma construtiva os erros, defeitos e falhas encontrados.

**Formas para melhorar a comunicação entre a pessoa de teste e os demais:**	
	• Começar com um espírito de colaboração, ao invés de conflitos, mostrando que todos tem o mesmo objetivo: melhorar a qualidade do sistema;
	• Comunicar de uma forma neutra os erros encontrados, focar no fato, sem criticar o autor;
	• Tentar compreender como a pessoa se sente ao receber a notícia e interpretar sua reação;
	• Confirmar se a outra pessoa entendeu o que você relatou, e vice-versa.


**Processo de teste - PDCA (Plan, Do, Check, Action)**	
	1. Definir a Meta;
	2. Definir o Método;
	3. Educar e treinar;
	4. Executar;
	5. Coletar dados;
	6. Checar;
	7. Ação: corretiva, preventiva e de melhoria.

---------------------------------------------------

# Fundamentos do processo de teste de software

Um processo de teste básico deve contemplar: 
	• Planejamento e controle; 
	• Análise e modelagem; 
	• Implementação e execução; 
	• Avaliação de critérios de saída e relatórios; 
	• Atividade de encerramento dos testes;
	• Melhoria/Corretiva/Preventiva. 
	

### Atividades de verificação e validação

Existem dois conceitos importantes no teste:

> Validação = Avaliação da veracidade do produto (baseado nos requisitos definidos pelo cliente). Deverá questionar se o que está sendo desenvolvido está correto, e se o sistema está de acordo com a especificação definida.

> Verificação = Avalia se o objeto foi desenvolvido da forma prevista, se o produto está seguindo o que foi combinado.

Ambos asseguram que o software esteja atendendo as necessidades e especificações pedidas pelo usuário.

-------------------------------------------

## Testes Funcionais

**Características:**	
	• Avaliam se o que está sendo construído está certo;
	• Avaliam o funcionamento da aplicação considerado o comportamento externo do software;
	• É um teste aplicável em todas as fases do teste (unitário, integração, sistema, aceitação);
	• Testa as funcionalidades, requerimentos, regras de negócios presentes na documentação.

**Como funciona?**
	• Dados de entrada são fornecidos >teste executado > resultado do teste comparado a um resultado esperado.
	

## Testes não Funcionais
Valida como o software está funcionando (desempenho, carga, stress, usabilidade...

## Testes Estruturais
Valida aspectos estruturais do software (cobertura do código, comandos, funções, decisão...

## Testes de Mudanças
	• Teste de confirmação (valida a remoção de defeitos);
	• Teste de regressão (executado quando o software ou o ambiente sofrem alterações; valida se não foram gerados novos defeitos).


# 1.2 Testes Unitários

	• Possui como objetivo testar a menor parte testável do sistema (unidade), que pode ser um módulo/objeto/classe;
	• É independente de outros testes, pois valida cada parte individualmente;
	• Caso exista dependência de métodos ou classes que não estão no teste, usa-se os mocks (objetos que simulam objetos reais)
	• O teste unitário também é caracterizado pelo uso de controladores (drivers) e simuladores (stubs)

### Tipos de níveis de testes 

	- TDD (Test Driven Development - Desenvolvimento orientado a testes): técnica de desenvolvimento de softwares em que primeiro é escrito o teste e só depois produzido um código para validá-lo;
	- Integração: Testa a integração entre os diversos componentes de software criados;
	

### Classificação dos testes 

**Técnica caixa-preta:**	
Não considera aspectos internos (código);

**Técnica caixa-branca**
Teste e cobertura de decisão
