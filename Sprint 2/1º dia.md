											
## 1. Como gerar qualidade no produto?

A atividade de testar engloba diversos artefatos que juntos geram a qualidade do produto, como:

	• Ter os requisitos atingidos;
	• Ter confiança;
	• Identificar defeitos;
	• Tomadas de decisão;
	• Reduzir riscos;
	• Conformidades contratuais e regulatórias.

### 1.1 E o que é testar?
Teste é o processo de explorar um software com o objetivo de encontrar defeitos. E não apenas isso, além de localizar os defeitos, é necessário definir o que acontecerá com eles.  
O teste deve ocorrer em todo o ciclo de vida do projeto, para assegurar que o software está em conformidade com o que foi especificado.  Dessa forma, teste pode ser feito pelo testador de forma manual ou automatizada. 

## 2. Tipos de Testes
As análises estáticas e dinâmicas estão entre as formas de buscar softwares com mais qualidade e segurança. Apesar de terem origens distintas, ambos podem ser levados para o ambiente de desenvolvimento. Dessa forma, podem ampliar a capacidade da companhia entregar produtos com menos erros e problemas de segurança.
Por ser feito logo nos estágios iniciais de desenvolvimento, os testes estáticos normalmente possuem um custo menor do que as análises dinâmicas. Por outro lado, um teste dinâmico pode ser executado mais rapidamente. Em ambos os casos, os métodos de análise são altamente complexos, capazes de verificar grandes sistemas com facilidade.
Esses procedimentos podem ser aplicados em qualquer empresa de desenvolvimento de sistemas. Lado a lado com boas práticas de desenvolvimento, eles ajudam a reduzir consideravelmente a quantidade de brechas e vulnerabilidades de um produto.

| Teste Estático |
|--|
| Trabalha diretamente no código sem a necessidade de executar o código; 
Utiliza o método white-box; Busca identificar erros de programação, como erros de sintaxe, 
falhas de segurança e práticas ruins; 
Necessita de revisão, inspeção e análise estática dos artefatos; 
Qualquer documento do projeto pode ser avaliado desta forma; 
Pode ser usado em todos os níveis de teste;
Verifica itens como: Código-fonte, Especificações de arquitetura, Estórias de usuário, Plano de projeto, Especificações de requisitos, Manual de usuário.  |  


|Teste dinâmico |
|--|
|Precisa que o software seja executado; 
Método black-box; 
É o mais utilizado no mercado; 
O custo tende a ser maior; 
Verifica itens como o tempo de resposta, a performance da aplicação, a capacidade do software em se adaptar em diferentes ambientes, o comportamento.|


### 2.1 Teste X Depuração
Sabemos que teste é o processo de explorar um software com o objetivo de encontrar defeitos e que deverá ocorrer em todo o ciclo de vida do projeto.
Após uma equipe de desenvolvimento receber um relatório da equipe de testes, se houver defeitos, eles começarão a depurar. **Depurar é o processo de consertar algo que se sabe que está quebrado. O objetivo é encontrar o bug e se livrar dele.**
O foco é o detalhe da execução, há uma preocupação com os algoritmos e as mudanças de estado. 

### 2.2 Teste é igual a qualidade?
O desafio do teste de software é alcançar a eficiência e a eficácia, portanto, o teste só aumenta a qualidade do software quando:

	• São encontrados defeitos;
	• Os defeitos são corrigidos;
	• Os requisitos não-funcionais (confiabilidade, usabilidade, escalabilidade e etc.,) são verificados.
	

Também passam pelo processo VV&T:

**2.3 Processo VV&T**

**Validação:** Assegurar que o produto final corresponda aos requisitos do usuário (estamos construindo o produto certo?)
	
**Verificação:** Assegurar a consistência, integridade e que corretitude do produto em cada fase e entre fases consecutivas do ciclo de vida do software (estamos construindo corretamente o produto?)
	
**Teste:** Examina o comportamento do produto por meio de sua execução.

Com os testes, o retrabalho, os custos de manutenção e os chamados de suporte são reduzidos. Ademais, cria-se um software bem estruturado, o que facilita novos projetos.

Ou seja, técnicas aplicadas com o nível apropriado de experiências em teste + as técnicas aplicadas nos pontos certos do ciclo de vida de desenvolvimento de software = redução da frequência de entregas problemáticas.


## 3. Erro, defeito, falha, engano... Quando utilizar cada um?

![image](https://user-images.githubusercontent.com/107884724/223719520-7f8d44a0-098f-4d9e-a6a9-65de4e3986c8.png)

Conforme a imagem, podemos concluir que:

- O **engano** introduz o defeito;
- O **defeito** produz um erro;
- O **erro** é mostrado para o usuário;
- Logo houve uma **falha**, que é a consequência do erro.
 

## 4. Os sete princípios dos testes

Exitem algumas diretrizes dos testes, que são:

**O teste mostra a presença de defeitos**
Testes conseguem identificar a existência de falhas, mas não pode garantir a ausência delas. Mesmo se nenhum erro for identificado em uma bateria de testes, não é possível afirmar que o software está livre de falhas.

**Testes exaustivos são impossíveis**
É necessário verificar os “riscos e prioridades” para focar aos esforços de testes nas principais expectativas e necessidades do software, já que testar “tudo” é praticamente impossível.

**O teste inicial economiza tempo e dinheiro**
As atividades de teste precisam iniciar o mais cedo possível no ciclo de vida do desenvolvimento;
Quanto mais cedo os testes começarem, maior a probabilidade de não ocorrer propagações de falha.

**Defeitos se agrupam**
Segue a definição do Princípio de Pareto: Um número pequeno de módulos (20%) contém a maioria dos defeitos descobertos (80%).

**Cuidado com o paradoxo do pesticida**
Os testes precisam ser regularmente atualizados, caso contrário eles se tornam ineficazes, tal qual um pesticida aplicado numa praga que já evoluiu e não é mais afetada por seus efeitos.

**O teste depende do contexto**
Cada contexto exige que a aplicação de testes seja diferente. Não é possível aplicar o mesmo teste de um sistema de segurança em um sistema de e-commerce.

**Ausência de erros é uma ilusão**
Independentemente de quantos defeitos foram encontrados e corrigidos, isso não significa necessariamente que os usuários estejam satisfeitos com o produto ou que ele atenderá ao seu propósito.


## 5. Fatores contextuais que influenciam o processo de teste

![image](https://user-images.githubusercontent.com/107884724/223720714-85dd8099-0ac9-4fcf-94a3-2aab9105a056.png)



## 6. Atividades de teste

![image](https://user-images.githubusercontent.com/107884724/223721544-f4137fb3-6e22-4807-97ca-f45889e36475.png)

**Planejamento do teste**	
- Define os propósitos e abordagem do teste;
- Criação do plano de teste (cronograma, exceções, recursos necessários);
- Define o escopo do teste;
- Seleciona as métricas;
- Determina o nível de detalhamento do teste.

**Análise do teste**
- Define as condições de teste associadas à base de teste analisada na etapa anterior.

**Modelagem do teste**
- Prioriza o conjunto de casos de teste;
- Identifica os dados de teste (massa de dados);
- Projeta o ambiente de teste.
- Elaborar os casos de teste com base nas condições de teste levantadas na tarefa anterior.

**Implementação do teste**
- Responde a pergunta "agora temos tudo para executar os testes?";
- Cria os scripts de testes automatizados;
- Cria a suíte de testes;
- Prepara os dados de teste e garante que sejam carregados corretamente no ambiente de teste;
	
**Os produtos de trabalho de implementação do teste incluem:**	• Os procedimentos de teste e seu sequenciamento;
- As suítes de teste;
- Um cronograma de execução do teste.

**Execução do teste**
- Os testes são feitos de acordo com o cronograma;
- Testes feitos manualmente;
- Colhem evidências, comparam os resultados com o que era esperado;
- Analisam as anomalias para achar as prováveis causas;
- Comunicam os defeitos;
- Registram o resultado da execução do teste;
- Executam o teste de confirmação e regressão;

**Conclusão do teste**
- Métricas consolidadas de encerramento dos testes;
- Lançamento do software;
- Verificar se todos os relatórios de defeitos estão fechados;
- Analisar lições aprendidas;
- Melhorar a maturidade dos processos.
	

## 7. A psicologia do teste
O desenvolvimento de software envolve pessoas, portanto, o fator psicológico influencia bastante em todo o processo.

![image](https://user-images.githubusercontent.com/107884724/223722968-fa87a47f-301a-4c04-96c3-73368473ba52.png)

Dessa forma, ao avaliar o trabalho do desenvolvedor um bom testador deve ter respeito, sensibilidade e ser atencioso com os outros ao fornecer feedback ou discutir falhas.
