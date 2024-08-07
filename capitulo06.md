# Capítulo 6 - Formatação de Texto

## Introdução

Bem-vindo ao capítulo sobre formatação de texto em HTML! Após aprendermos sobre a estrutura básica de documentos HTML e como usar títulos e parágrafos, é hora de explorarmos as diversas maneiras de formatar o texto dentro desses elementos. A formatação adequada não apenas melhora a aparência do seu conteúdo, mas também ajuda a transmitir significado e ênfase, melhorando a compreensão do leitor e a acessibilidade do site.

Neste capítulo, vamos cobrir uma variedade de elementos HTML usados para formatar texto, desde negrito e itálico até elementos mais específicos como citações e código. Lembre-se de que, embora o HTML forneça estas opções de formatação, o estilo visual final geralmente é controlado pelo CSS.

## 6.1 Ênfase e Importância

### 6.1.1 Texto em Itálico (`<em>`)

O elemento `<em>` é usado para dar ênfase ao texto. Por padrão, os navegadores exibem este texto em itálico.

```html
<p>Eu <em>realmente</em> gosto de desenvolvimento web.</p>
```

### 6.1.2 Texto em Negrito (`<strong>`)

O elemento `<strong>` é usado para indicar forte importância. Os navegadores geralmente exibem este texto em negrito.

```html
<p>É <strong>crucial</strong> entender HTML para desenvolvimento web.</p>
```

### 6.1.3 Combinando Ênfase e Importância

Você pode combinar `<em>` e `<strong>` para maior ênfase:

```html
<p>Este é um ponto <strong><em>extremamente importante</em></strong>.</p>
```

## 6.2 Elementos Puramente Estilísticos

Embora `<em>` e `<strong>` sejam preferidos por seu valor semântico, existem elementos puramente estilísticos:

### 6.2.1 Itálico (`<i>`)

```html
<p>O termo <i>Homo sapiens</i> significa "homem sábio" em latim.</p>
```

### 6.2.2 Negrito (`<b>`)

```html
<p>Não se esqueça de clicar no botão <b>Salvar</b> antes de sair.</p>
```

## 6.3 Sublinhado e Tachado

### 6.3.1 Sublinhado (`<u>`)

O elemento `<u>` é usado para sublinhar texto, mas deve ser usado com cautela, pois pode ser confundido com links.

```html
<p>Isso é um <u>texto sublinhado</u>.</p>
```

### 6.3.2 Tachado (`<s>`)

O elemento `<s>` representa texto que não é mais relevante ou preciso.

```html
<p>O preço era <s>R$50,00</s>, agora é R$40,00.</p>
```

## 6.4 Sobrescrito e Subscrito

### 6.4.1 Sobrescrito (`<sup>`)

Usado para caracteres que devem aparecer acima da linha de base.

```html
<p>A fórmula da água é H<sup>2</sup>O.</p>
```

### 6.4.2 Subscrito (`<sub>`)

Usado para caracteres que devem aparecer abaixo da linha de base.

```html
<p>O símbolo químico do cobre é Cu<sub>29</sub>.</p>
```

## 6.5 Citações

### 6.5.1 Citações em Bloco (`<blockquote>`)

Para citações longas que formam um parágrafo próprio.

```html
<blockquote>
    <p>A web é mais uma criação social do que técnica. Eu a construí para um efeito social – para ajudar as pessoas a trabalharem juntas – e não como um brinquedo técnico.</p>
    Tim Berners-Lee
</blockquote>
```

### 6.5.2 Citações Inline (`<q>`)

Para citações curtas dentro de um parágrafo.

```html
<p>Como Steve Jobs disse, <q>A inovação distingue entre um líder e um seguidor.</q></p>
```

## 6.6 Abreviações e Acrônimos

O elemento `<abbr>` é usado para especificar abreviações e acrônimos.

```html
<p>A <abbr title="World Wide Web">WWW</abbr> foi inventada por Tim Berners-Lee.</p>
```

## 6.7 Código e Saída de Computador

### 6.7.1 Código Inline (`<code>`)

Para pequenos trechos de código dentro de um texto.

```html
<p>Use a função <code>console.log()</code> para depurar em JavaScript.</p>
```

### 6.7.2 Bloco de Código (`<pre>`)

Para blocos maiores de código, preservando espaços e quebras de linha.

```html
<pre><code>
function saudacao(nome) {
    console.log("Olá, " + nome + "!");
}
</code></pre>
```

### 6.7.3 Saída de Computador (`<samp>`)

Para representar a saída de um programa de computador.

```html
<p>O programa retornou: <samp>Erro 404: Arquivo não encontrado</samp></p>
```

## 6.8 Marcação e Destaque

### 6.8.1 Texto Marcado (`<mark>`)

Para destacar partes do texto, geralmente exibido com um fundo amarelo.

```html
<p>Neste texto, <mark>esta parte é importante</mark> e deve ser notada.</p>
```

## 6.9 Definições e Termos Técnicos

### 6.9.1 Definição (`<dfn>`)

Para marcar a ocorrência de definição de um termo.

```html
<p><dfn>HTML</dfn> é a linguagem de marcação padrão para criar páginas web.</p>
```

## Conclusão

A formatação de texto em HTML oferece uma ampla gama de opções para estruturar e enfatizar seu conteúdo. Ao usar esses elementos corretamente, você não apenas melhora a aparência visual do seu texto, mas também adiciona significado semântico, o que é crucial para acessibilidade e SEO.

Lembre-se de que, embora o HTML forneça estas opções de formatação, o estilo visual final deve ser controlado principalmente através do CSS. O HTML deve se concentrar na estrutura e no significado do conteúdo, enquanto o CSS cuida da apresentação.

Exercício prático: Crie uma página HTML que utilize vários dos elementos de formatação de texto que aprendemos neste capítulo. Experimente com diferentes combinações e observe como elas afetam a aparência e o significado do seu conteúdo. Tente criar um artigo curto ou uma página informativa que faça uso efetivo desses elementos para melhorar a legibilidade e a estrutura do texto.

No próximo capítulo, exploraremos como criar e formatar listas em HTML, outro aspecto fundamental da estruturação de conteúdo em páginas web.