# Fundamentos do teste de software (back-end)

## Por que é importante testar?
A partir da construção do projeto são implementados os testes. Os testes agregam valor ao projetos pois conseguem encontrar os erros de forma antecipada.
Sendo assim, como os testes influenciam na vida do software?

## Pirâmide de testes
### Testes de Unidade
Os testes de unidade (unit) verificam o funcionamento da menor unidade de código testável da aplicação. Geralmente é vista como um método público em uma classe, mas também pode ser vista como um conjunto de classes/métodos/objetos interagindo entre si.
Além de pequenos (por testarem apenas uma partezinha do sistema), os testes de unidade são independentes de colaboradores externos à unidade. São vantajosos pois são simples e fáceis de rodar, além de ajudar a saber exatamente onde está um possível problema.

### Testes de integração
Imagine que você testou duas unidades separadas, e elas estão funcionando perfeitamente. Porém, ao colocar essas duas unidades juntas o resultado não foi positivo: elas não rodam. Para resolver esse problema existem os testes de integração, que testam algumas unidades funcionando em conjunto.
Características:
	• Testam as funcionalidades, e não o sistema como um todo;
	• São mais complicados de fazer e manter, são mais demorados que os testes de unidade;
	• Porém são mais simples de fazer e manter -além de mais rápidos- se comparado aos testes de ponta a ponta, pois testam uma única funcionalidade de cada vez.


### Testes de ponta a ponta (E2E)
Características:
	• Simulam um ambiente real (abrem navegador, preenchem formulários, clicam em botões, etc);
	• Os testes acontecem em um ambiente controlado;
	• Quem executa as ações é um robozinho;
	• São testes complexos de escrever e costumam demorar um tempo considerável para rodar.

**Exemplo de ciclo de teste E2E** 
Objetivo: verificar como está sendo uma compra online no app da marca XYZ.
Passos:
	1. Cadastrar
	2. Escolher item
	3. Calcular frete
	4. Sacola
	5. Pagamento
	6. Finalizar pedido
	7. Informações do pedido
	8. Boleto
	9. Meus pedidos
