# Capítulo 10 - Tabelas

## Introdução

Bem-vindo ao capítulo sobre tabelas em HTML! As tabelas são uma ferramenta poderosa para apresentar dados estruturados de forma organizada e compreensível. Embora não devam ser usadas para layout de página (uma prática comum no passado), as tabelas continuam sendo essenciais para exibir informações tabulares, como dados estatísticos, horários, comparações de produtos e muito mais.

Neste capítulo, aprenderemos como criar tabelas em HTML, estruturá-las corretamente, estilizá-las com CSS e garantir que sejam acessíveis para todos os usuários. Vamos explorar os elementos básicos de tabelas, técnicas avançadas e melhores práticas para seu uso efetivo.

## 10.1 Estrutura Básica de uma Tabela

Uma tabela em HTML é composta por vários elementos:

- `<table>`: O elemento principal que define a tabela.
- `<tr>`: Define uma linha da tabela (table row).
- `<td>`: Define uma célula de dados da tabela (table data).
- `<th>`: Define uma célula de cabeçalho da tabela (table header).

Exemplo básico:

```html
<table>
  <tr>
    <th>Cabeçalho 1</th>
    <th>Cabeçalho 2</th>
  </tr>
  <tr>
    <td>Dado 1</td>
    <td>Dado 2</td>
  </tr>
  <tr>
    <td>Dado 3</td>
    <td>Dado 4</td>
  </tr>
</table>
```

## 10.2 Cabeçalhos de Tabela

Usar `<th>` para cabeçalhos é importante para a estrutura e acessibilidade da tabela:

```html
<table>
  <tr>
    <th>Nome</th>
    <th>Idade</th>
    <th>Profissão</th>
  </tr>
  <tr>
    <td>João</td>
    <td>30</td>
    <td>Engenheiro</td>
  </tr>
  <tr>
    <td>Maria</td>
    <td>28</td>
    <td>Advogada</td>
  </tr>
</table>
```

## 10.3 Elementos Semânticos de Tabela

Para melhorar a estrutura e o significado da tabela, use:

- `<thead>`: Agrupa o conteúdo do cabeçalho da tabela.
- `<tbody>`: Agrupa o conteúdo do corpo da tabela.
- `<tfoot>`: Agrupa o conteúdo do rodapé da tabela.

Exemplo:

```html
<table>
  <thead>
    <tr>
      <th>Produto</th>
      <th>Preço</th>
    </tr>
  </thead>
  <tbody>
    <tr>
      <td>Maçã</td>
      <td>R$ 2,00</td>
    </tr>
    <tr>
      <td>Banana</td>
      <td>R$ 3,00</td>
    </tr>
  </tbody>
  <tfoot>
    <tr>
      <td>Total</td>
      <td>R$ 5,00</td>
    </tr>
  </tfoot>
</table>
```

## 10.4 Mesclagem de Células

Você pode mesclar células usando os atributos `colspan` e `rowspan`:

```html
<table>
  <tr>
    <th colspan="2">Dados Pessoais</th>
  </tr>
  <tr>
    <td>Nome</td>
    <td>João Silva</td>
  </tr>
  <tr>
    <td>Endereço</td>
    <td>Rua das Flores, 123</td>
  </tr>
</table>
```

## 10.5 Acessibilidade em Tabelas

Para melhorar a acessibilidade:

1. Use o atributo `scope` em células de cabeçalho:

```html
<th scope="col">Nome</th>
<th scope="col">Idade</th>
```

2. Adicione uma descrição com `<caption>`:

```html
<table>
  <caption>Lista de Funcionários</caption>
  <!-- conteúdo da tabela -->
</table>
```

3. Use `headers` e `id` para associar dados a cabeçalhos em tabelas complexas:

```html
<table>
  <tr>
    <th id="nome">Nome</th>
    <th id="idade">Idade</th>
  </tr>
  <tr>
    <td headers="nome">João</td>
    <td headers="idade">30</td>
  </tr>
</table>
```

## 10.6 Estilização de Tabelas com CSS

CSS pode melhorar significativamente a aparência das tabelas:

```html
<style>
  table {
    border-collapse: collapse;
    width: 100%;
  }
  th, td {
    border: 1px solid #ddd;
    padding: 8px;
    text-align: left;
  }
  th {
    background-color: #f2f2f2;
  }
  tr:nth-child(even) {
    background-color: #f9f9f9;
  }
</style>
```

## 10.7 Tabelas Responsivas

Para tabelas responsivas em dispositivos móveis, você pode usar um wrapper com overflow:

```html
<style>
  .table-responsive {
    overflow-x: auto;
  }
</style>

<div class="table-responsive">
  <table>
    <!-- conteúdo da tabela -->
  </table>
</div>
```

## 10.8 Tabelas para Layouts (Não Recomendado)

Embora as tabelas tenham sido usadas no passado para layouts de página, esta prática não é mais recomendada. Use CSS flexbox ou grid para layouts modernos e responsivos.

## 10.9 Boas Práticas para Tabelas

1. Use tabelas apenas para dados tabulares, não para layout.
2. Mantenha as tabelas simples e use cabeçalhos claros.
3. Use `<thead>`, `<tbody>`, e `<tfoot>` para estrutura semântica.
4. Forneça uma `<caption>` para descrever o conteúdo da tabela.
5. Use CSS para estilização, não atributos HTML obsoletos como `cellpadding`.
6. Considere alternativas para dispositivos móveis, como cards ou listas para dados complexos.

## 10.10 Exemplo Avançado de Tabela

Aqui está um exemplo que incorpora muitas das técnicas discutidas:

```html
<style>
  table {
    border-collapse: collapse;
    width: 100%;
  }
  th, td {
    border: 1px solid #ddd;
    padding: 8px;
    text-align: left;
  }
  th {
    background-color: #4CAF50;
    color: white;
  }
  tr:nth-child(even) {
    background-color: #f2f2f2;
  }
  caption {
    font-weight: bold;
    margin-bottom: 10px;
  }
</style>

<div class="table-responsive">
  <table>
    <caption>Relatório de Vendas Trimestrais</caption>
    <thead>
      <tr>
        <th scope="col">Produto</th>
        <th scope="col">Q1</th>
        <th scope="col">Q2</th>
        <th scope="col">Q3</th>
        <th scope="col">Q4</th>
      </tr>
    </thead>
    <tbody>
      <tr>
        <th scope="row">Produto A</th>
        <td>100</td>
        <td>150</td>
        <td>200</td>
        <td>250</td>
      </tr>
      <tr>
        <th scope="row">Produto B</th>
        <td>200</td>
        <td>250</td>
        <td>300</td>
        <td>350</td>
      </tr>
    </tbody>
    <tfoot>
      <tr>
        <th scope="row">Total</th>
        <td>300</td>
        <td>400</td>
        <td>500</td>
        <td>600</td>
      </tr>
    </tfoot>
  </table>
</div>
```

## Conclusão

As tabelas HTML são uma ferramenta poderosa para apresentar dados estruturados. Quando usadas corretamente, elas podem melhorar significativamente a compreensão e a acessibilidade das informações em sua página web. Lembre-se de usar tabelas apenas para dados tabulares, aproveitar elementos semânticos, e considerar a responsividade e acessibilidade em seu design.

Exercício prático: Crie uma tabela complexa com múltiplas linhas e colunas, incluindo cabeçalhos de linha e coluna. Use `colspan` e `rowspan` para mesclar algumas células. Aplique estilos CSS para melhorar a aparência da tabela e torne-a responsiva. Certifique-se de incluir elementos semânticos como `<thead>`, `<tbody>`, e `<tfoot>`, e adicione uma `<caption>` descritiva.

No próximo capítulo, exploraremos formulários HTML, um componente crucial para interação do usuário e coleta de dados em websites.