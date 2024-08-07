# Capítulo 2 - Estrutura básica de um documento HTML

## Introdução

Após compreendermos o que é HTML e sua importância no desenvolvimento web, é hora de mergulharmos na estrutura fundamental de um documento HTML. Neste capítulo, exploraremos os elementos essenciais que compõem a base de qualquer página web, fornecendo uma compreensão sólida sobre como organizar seu código HTML de maneira eficiente e semântica.

## 2.1 A Anatomia de um Documento HTML

Todo documento HTML segue uma estrutura básica que serve como esqueleto para o conteúdo da página. Esta estrutura consiste em vários elementos-chave que trabalham juntos para criar uma página web funcional e bem organizada.

Vamos examinar um exemplo simples de um documento HTML:

```html
<!DOCTYPE html>
<html lang="pt-BR">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página Web</title>
</head>
<body>
    <h1>Bem-vindo à Minha Página</h1>
    <p>Este é um parágrafo de exemplo.</p>
</body>
</html>
```

Agora, vamos dissecar cada parte deste documento.

## 2.2 Declaração DOCTYPE

```html
<!DOCTYPE html>
```

A declaração DOCTYPE é a primeira linha de um documento HTML. Ela informa ao navegador que este é um documento HTML5, o padrão atual para HTML. Esta declaração é crucial para garantir que o navegador renderize a página corretamente.

## 2.3 O Elemento HTML

```html
<html lang="pt-BR">
```

O elemento `<html>` é o elemento raiz de um documento HTML. Ele envolve todo o conteúdo da página. O atributo `lang` especifica o idioma do documento, o que é importante para acessibilidade e SEO.

## 2.4 O Elemento Head

```html
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>Minha Página Web</title>
</head>
```

O elemento `<head>` contém metadados sobre o documento HTML. Estes são informações que não são diretamente visíveis na página, mas são cruciais para seu funcionamento correto. Vamos detalhar os elementos dentro do `<head>`:

### 2.4.1 Meta Charset

```html
<meta charset="UTF-8">
```

Esta tag define o conjunto de caracteres usado no documento. UTF-8 é o padrão recomendado, pois suporta praticamente todos os caracteres e símbolos.

### 2.4.2 Meta Viewport

```html
<meta name="viewport" content="width=device-width, initial-scale=1.0">
```

Esta meta tag é essencial para design responsivo. Ela instrui o navegador sobre como controlar as dimensões e o escalonamento da página em dispositivos móveis.

### 2.4.3 Título do Documento

```html
<title>Minha Página Web</title>
```

O elemento `<title>` define o título da página, que aparece na aba do navegador e nos resultados de busca. É crucial para SEO e usabilidade.

## 2.5 O Elemento Body

```html
<body>
    <h1>Bem-vindo à Minha Página</h1>
    <p>Este é um parágrafo de exemplo.</p>
</body>
```

O elemento `<body>` contém todo o conteúdo visível da página web, como texto, imagens, links, etc. É aqui que a maior parte do seu HTML será escrito.

## 2.6 Hierarquia e Aninhamento

É importante entender que os elementos HTML seguem uma estrutura hierárquica. Elementos podem conter outros elementos, criando um aninhamento. Por exemplo:

```html
<body>
    <header>
        <h1>Título Principal</h1>
        <nav>
            <ul>
                <li><a href="#home">Home</a></li>
                <li><a href="#sobre">Sobre</a></li>
            </ul>
        </nav>
    </header>
    <main>
        <article>
            <h2>Artigo</h2>
            <p>Conteúdo do artigo...</p>
        </article>
    </main>
    <footer>
        <p>&copy; 2024 Minha Empresa</p>
    </footer>
</body>
```

Este exemplo mostra como elementos podem ser aninhados para criar uma estrutura semântica e organizada.

## 2.7 Comentários em HTML

Comentários são úteis para documentar seu código e são ignorados pelos navegadores. Eles são escritos assim:

```html
<!-- Este é um comentário em HTML -->
```

## Conclusão

Compreender a estrutura básica de um documento HTML é fundamental para qualquer desenvolvedor web. Esta estrutura serve como a fundação sobre a qual você construirá páginas web mais complexas e interativas. Ao dominar estes elementos básicos, você estará bem preparado para explorar aspectos mais avançados do HTML nos capítulos seguintes.
