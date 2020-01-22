# Teste Prático

O objetivo deste teste é conhecer suas habilidades em:

* Desenvolvimento Web (Tecnologias, Linguagens de programação, Frameworks, Banco de Dados, HTML, CSS e JavaScript);
* Entendimento e análise dos requisitos;
* Modelagem de banco de dados;
* Integração com WebServices;

Você deve desenvolver uma pequena aplicação WEB utilizando a linguagem de programação, framework(s) e banco de dados relacional de sua preferência.

## Problema

### Portal de Vendas

* Um vendedor quer registrar as vendas de produtos para seus clientes;
* O registro de uma venda deve conter: Número da Venda, Cliente, Data da Venda, Total da Venda, Itens Vendidos (Número, Produto, Quantidade, Preço e Total), CEP e Endereço de Entrega;
* Deve ser possível visualizar uma lista com vendas registradas (Número, Data da Venda, Cliente, Total da Venda);
* No cadastro da venda deve ser possível: buscar clientes pelo nome e buscar os produtos pelo nome;
* Ao adicionar um Item a uma Venda, deve-se listar o Número do Item, o Produto (Código e Descrição), o Preço, a Quantidade e o Total do Item;
* O Total da Venda deve ser atualizado a cada item adicionado;
* Campo Endereço de Entrega deve ser preenchido automaticamente ao informar o CEP de Entrega;
* Exemplo da página de Registro de Vendas:

```
| Número da Venda | 000001
|   Data da Venda | 19/01/2020
|         Cliente | Cliente A
|  CEP de Entrega | 37925-000
|     End.Entrega | logradouro, complemento, bairro, localidade, uf

|----------|-------------|--------------|--------|------------|-------|
| Núm.Item | Cód.Produto | Desc.Produto | Preço  | Quantidade | Total |
|----------|-------------|--------------|--------|------------|-------|
|      001 |        0002 | Prod A       |   3,20 |     10,000 | 32,00 |
|      002 |        0017 | Prod B       |   1,30 |     10,000 | 13,00 |
|      003 |        0004 | Prod C       |   5,80 |     10,000 | 58,00 |
|----------|-------------|--------------|--------|------------|-------|

|Total| 103,00
```

* Exemplo da página com a Lista das Vendas:

```
| Relação de Vendas |

|-----------|------------|--------------|--------|
| Núm.Venda | Data Venda | Cliente      | Total  | 
|-----------|------------|--------------|--------|
|    000001 | 19/01/2020 | Cliente A    | 103,00 |
|    000002 | 20/01/2020 | Cliente B    | 411,30 |
|    000003 | 20/01/2020 | Cliente C    | 285,80 |
|-----------|------------|--------------|--------|
```

## Orientações

* Nesta aplicação é necessário desenvolver apenas duas páginas, uma para listar as vendas cadastradas e outra para realizar o cadastro das vendas;
* Não é necessário implementar o cadastro de produtos e clientes, somente suas tabelas no banco de dados. Popule essas diretamente no banco de dados;
* O cadastro de produtos deve conter: código e descrição;
* O cadastro de clientes deve conter: código nome e cnpj; 
* O banco de dados não pode permitir 2 produtos com o mesmo código;
* O campo Número da Venda deve ser sequencial e gerado automaticamente;
* O campo Número do Item deve ser sequencial e gerado automaticamente;
* Deve usar o webservice da ViaCEP (https://viacep.com.br/) para preencher o endereço após preencher o campo CEP;
* Faça fork desse projeto e edite este README explicando como executar e testar a aplicação;
* Todos os arquivos necessários para rodar o projeto devem estar no repositório do github;


## Diferenciais

* Testes unitários para qualquer parte do sistema;
* Comentários claros no código;
* Procure fazer vários commits com mensagens claras;
