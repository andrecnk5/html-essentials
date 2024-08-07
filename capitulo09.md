# Capítulo 9 - Imagens

## Introdução

Bem-vindo ao capítulo sobre imagens em HTML! As imagens são elementos essenciais no design web moderno, tornando as páginas mais atrativas, informativas e envolventes. Neste capítulo, exploraremos como incorporar imagens em suas páginas HTML, otimizá-las para web e garantir que sejam acessíveis para todos os usuários.

Aprenderemos sobre a tag `<img>`, seus atributos importantes, formatos de imagem para web, técnicas de otimização e as melhores práticas para uso de imagens em design responsivo.

## 9.1 A Tag `<img>`

A tag `<img>` é usada para incorporar imagens em uma página HTML. É uma tag de fechamento automático, o que significa que não precisa de uma tag de fechamento separada.

Sintaxe básica:

```html
<img src="caminho/para/imagem.jpg" alt="Descrição da imagem">
```

### 9.1.1 Atributos Essenciais

1. **src**: Especifica o caminho para o arquivo de imagem.
2. **alt**: Fornece uma descrição textual da imagem para acessibilidade e SEO.

Exemplo:

```html
<img src="gato.jpg" alt="Um gato laranja sentado em um sofá">
```

## 9.2 Formatos de Imagem para Web

Os formatos mais comuns para imagens na web são:

1. **JPEG (.jpg, .jpeg)**: Ideal para fotografias e imagens com muitas cores.
2. **PNG (.png)**: Melhor para imagens com transparência ou com poucas cores.
3. **GIF (.gif)**: Usado para animações simples e imagens com poucas cores.
4. **WebP (.webp)**: Formato moderno que oferece boa compressão para imagens estáticas e animadas.
5. **SVG (.svg)**: Ideal para logos, ícones e gráficos que precisam ser escalados.

Exemplo de uso de SVG:

```html
<img src="logo.svg" alt="Logo da Empresa" width="100" height="100">
```

## 9.3 Dimensionamento de Imagens

Você pode especificar as dimensões da imagem usando os atributos `width` e `height`:

```html
<img src="foto.jpg" alt="Paisagem" width="500" height="300">
```

É uma boa prática especificar estas dimensões para ajudar o navegador a reservar espaço para a imagem antes de carregá-la, reduzindo o layout shift.

## 9.4 Imagens Responsivas

Para criar imagens que se adaptem a diferentes tamanhos de tela, você pode usar:

### 9.4.1 Atributo `srcset`

Permite especificar múltiplas versões da mesma imagem para diferentes resoluções:

```html
<img src="imagem-pequena.jpg"
     srcset="imagem-pequena.jpg 300w,
             imagem-media.jpg 600w,
             imagem-grande.jpg 1200w"
     sizes="(max-width: 600px) 300px,
            (max-width: 1200px) 600px,
            1200px"
     alt="Descrição da imagem">
```

### 9.4.2 Tag `<picture>`

Permite especificar diferentes imagens para diferentes condições:

```html
<picture>
    <source media="(min-width: 800px)" srcset="imagem-grande.jpg">
    <source media="(min-width: 400px)" srcset="imagem-media.jpg">
    <img src="imagem-pequena.jpg" alt="Descrição da imagem">
</picture>
```

## 9.5 Otimização de Imagens

Otimizar imagens é crucial para o desempenho do site:

1. **Comprima imagens**: Use ferramentas como TinyPNG ou ImageOptim.
2. **Escolha o formato correto**: JPEG para fotos, PNG para imagens com transparência, SVG para gráficos vetoriais.
3. **Use tamanhos apropriados**: Não carregue imagens maiores do que o necessário.
4. **Implemente carregamento lazy**: Carregue imagens apenas quando necessário.

Exemplo de lazy loading:

```html
<img src="imagem.jpg" alt="Descrição" loading="lazy">
```

## 9.6 Acessibilidade em Imagens

### 9.6.1 Uso Adequado do Atributo `alt`

O atributo `alt` é crucial para a acessibilidade:

```html
<img src="grafico-vendas.png" alt="Gráfico mostrando aumento de vendas em 20% no último trimestre">
```

Para imagens decorativas que não adicionam conteúdo, use um `alt` vazio:

```html
<img src="decoracao.png" alt="">
```

### 9.6.2 Imagens Complexas

Para imagens complexas, use `aria-describedby` para fornecer uma descrição mais detalhada:

```html
<img src="diagrama-complexo.png" alt="Diagrama do processo de produção" aria-describedby="desc-diagrama">
<p id="desc-diagrama">Este diagrama ilustra o processo de produção em 5 etapas: preparação, montagem, teste, embalagem e expedição.</p>
```

## 9.7 Figuras e Legendas

Use `<figure>` e `<figcaption>` para associar imagens com legendas:

```html
<figure>
    <img src="foto-historica.jpg" alt="Fotografia da primeira loja da empresa em 1950">
    <figcaption>Nossa primeira loja, inaugurada em 1950 no centro da cidade.</figcaption>
</figure>
```

## 9.8 Mapas de Imagem

Mapas de imagem permitem criar áreas clicáveis dentro de uma imagem:

```html
<img src="mapa.jpg" alt="Mapa do escritório" usemap="#mapa-escritorio">
<map name="mapa-escritorio">
    <area shape="rect" coords="34,44,270,350" alt="Sala de Reuniões" href="sala-reunioes.html">
    <area shape="circle" coords="337,300,44" alt="Cafeteria" href="cafeteria.html">
</map>
```

## 9.9 Imagens de Fundo com CSS

Às vezes, é mais apropriado usar imagens como plano de fundo via CSS:

```html
<style>
    .header-bg {
        background-image: url('header-bg.jpg');
        background-size: cover;
        height: 200px;
    }
</style>
<div class="header-bg"></div>
```

## Conclusão

As imagens são componentes vitais do design web moderno, capazes de transmitir informações, evocar emoções e melhorar significativamente a experiência do usuário. Ao usar imagens em HTML, é importante considerar não apenas a estética, mas também o desempenho, a acessibilidade e a responsividade.

Lembre-se sempre de otimizar suas imagens, fornecer alternativas textuais adequadas e implementar técnicas responsivas para garantir que suas imagens sejam eficazes em todos os dispositivos e acessíveis a todos os usuários.

Exercício prático: Crie uma página HTML que demonstre o uso de vários tipos de imagens. Inclua uma imagem responsiva usando `srcset`, uma figura com legenda, um mapa de imagem e uma imagem de fundo CSS. Pratique a otimização de imagens e certifique-se de que todas as imagens tenham descrições alt apropriadas.

No próximo capítulo, exploraremos como criar e estilizar tabelas em HTML, uma ferramenta poderosa para apresentar dados estruturados em suas páginas web.