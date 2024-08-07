# Capítulo 3 - Tags e elementos HTML

## Introdução

Bem-vindo ao coração do HTML! Neste capítulo, mergulharemos no mundo das tags e elementos HTML, os blocos de construção fundamentais de qualquer página web. Compreender como usar tags e elementos corretamente é essencial para criar estruturas web bem organizadas e semanticamente significativas. Vamos explorar os conceitos básicos, a sintaxe e os usos comuns de várias tags HTML.

## 3.1 O que são Tags e Elementos HTML?

### Tags HTML

Tags são os marcadores usados para definir a estrutura e o conteúdo de uma página web. Elas são escritas entre colchetes angulares `< >` e geralmente vêm em pares: uma tag de abertura e uma tag de fechamento.

Exemplo:
```html
<p>Este é um parágrafo.</p>
```

Neste exemplo, `<p>` é a tag de abertura e `</p>` é a tag de fechamento.

### Elementos HTML

Um elemento HTML consiste em uma tag de abertura, o conteúdo e uma tag de fechamento. O elemento completo no exemplo acima é:

```html
<p>Este é um parágrafo.</p>
```

O elemento inteiro inclui as tags e o conteúdo entre elas.

## 3.2 Anatomia de uma Tag HTML

Uma tag HTML típica consiste em:

1. Colchetes angulares `< >`
2. Nome da tag (como "p" para parágrafo, "h1" para cabeçalho de nível 1, etc.)
3. Atributos (opcionais, discutiremos mais sobre isso em um capítulo posterior)
4. Conteúdo (entre as tags de abertura e fechamento)
5. Tag de fechamento (com uma barra `/` antes do nome da tag)

Exemplo com atributo:
```html
<a href="https://www.exemplo.com">Clique aqui</a>
```

Neste exemplo, `href` é um atributo que especifica o URL do link.

## 3.3 Tags de Abertura e Fechamento

A maioria das tags HTML vem em pares:

- Tag de abertura: `<tag>`
- Tag de fechamento: `</tag>`

Exemplo:
```html
<h1>Este é um título principal</h1>
<p>Este é um parágrafo de texto.</p>
```

## 3.4 Elementos Vazios

Alguns elementos HTML não têm conteúdo e, portanto, não precisam de uma tag de fechamento. Estes são chamados de elementos vazios ou self-closing tags.

Exemplos:
```html
<br> <!-- quebra de linha -->
<img src="imagem.jpg" alt="Descrição da imagem"> <!-- imagem -->
<input type="text"> <!-- campo de entrada -->
```

Em HTML5, você pode opcionalmente fechar estes elementos assim: `<br />`, `<img ... />`, mas isso não é obrigatório.

## 3.5 Aninhamento de Elementos

Elementos HTML podem ser aninhados uns dentro dos outros. Isso cria uma estrutura hierárquica em sua página web.

Exemplo:
```html
<div>
    <h1>Título Principal</h1>
    <p>Este é um parágrafo com <strong>texto em negrito</strong> e <em>texto em itálico</em>.</p>
</div>
```

É importante fechar as tags na ordem correta para manter uma estrutura adequada.

## 3.6 Elementos de Bloco vs. Elementos Inline

HTML tem dois tipos principais de elementos:

### Elementos de Bloco

Elementos de bloco começam em uma nova linha e ocupam toda a largura disponível.

Exemplos:
- `<div>`
- `<p>`
- `<h1>` a `<h6>`
- `<ul>` e `<ol>`

### Elementos Inline

Elementos inline não começam em uma nova linha e só ocupam o espaço necessário.

Exemplos:
- `<span>`
- `<a>`
- `<strong>`
- `<em>`

## 3.7 Tags HTML Comuns e Seus Usos

Vamos explorar algumas das tags HTML mais comuns:

1. Títulos e Subtítulos:
   ```html
   <h1>Título Principal</h1>
   <h2>Subtítulo</h2>
   <h3>Sub-subtítulo</h3>
   <!-- ... até h6 -->
   ```

2. Parágrafos:
   ```html
   <p>Este é um parágrafo de texto.</p>
   ```

3. Links:
   ```html
   <a href="https://www.exemplo.com">Clique aqui</a>
   ```

4. Imagens:
   ```html
   <img src="imagem.jpg" alt="Descrição da imagem">
   ```

5. Listas:
   ```html
   <ul>
     <li>Item não ordenado 1</li>
     <li>Item não ordenado 2</li>
   </ul>
   
   <ol>
     <li>Item ordenado 1</li>
     <li>Item ordenado 2</li>
   </ol>
   ```

6. Ênfase e Destaque:
   ```html
   <em>Texto em itálico</em>
   <strong>Texto em negrito</strong>
   ```

7. Divisões e Seções:
   ```html
   <div>Uma divisão genérica</div>
   <section>Uma seção de conteúdo</section>
   ```

## Conclusão

Compreender tags e elementos HTML é fundamental para criar estruturas web eficazes e significativas. À medida que você se familiariza com estas tags básicas, poderá começar a criar páginas mais complexas e expressivas.

Lembre-se, a prática é essencial. Experimente com diferentes tags, aninhando-as de várias maneiras, e veja como elas afetam a estrutura e a aparência de sua página web. No próximo capítulo, exploraremos mais profundamente os atributos HTML, que nos permitem adicionar informações extras e funcionalidades às nossas tags.

Exercício prático: Tente criar uma página HTML simples usando várias das tags que aprendemos neste capítulo. Inclua títulos, parágrafos, listas e links. Isso ajudará a solidificar seu entendimento e lhe dará experiência prática na estruturação de conteúdo web.