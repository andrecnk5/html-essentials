# Capítulo 11: Formulários HTML

## Introdução

Os formulários são componentes essenciais da web interativa, permitindo que os usuários insiram dados e os enviem para processamento. Eles são a ponte entre o usuário e o servidor, facilitando a coleta de informações, pesquisas, login de usuários e muito mais. Neste capítulo, exploraremos a criação e o uso de formulários em HTML, seus diversos elementos e as melhores práticas para implementá-los.

## 11.1 A tag `<form>`

A base de qualquer formulário HTML é a tag `<form>`. Esta tag envolve todos os elementos do formulário e define suas propriedades básicas.

### Exemplo básico:

```html
<form action="/submit-form" method="POST">
  <!-- Elementos do formulário vão aqui -->
</form>
```

### Atributos importantes:

- `action`: Especifica para onde os dados do formulário serão enviados.
- `method`: Define o método HTTP a ser usado (geralmente GET ou POST).

## 11.2 Elementos de entrada

Os elementos de entrada são o coração do formulário, permitindo que os usuários insiram diversos tipos de dados.

### 11.2.1 A tag `<input>`

A tag `<input>` é versátil e pode criar vários tipos de campos de entrada.

#### Exemplos:

```html
<!-- Campo de texto -->
<input type="text" name="username" placeholder="Digite seu nome de usuário">

<!-- Campo de senha -->
<input type="password" name="password" placeholder="Digite sua senha">

<!-- Caixa de seleção -->
<input type="checkbox" name="newsletter" id="newsletter">
<label for="newsletter">Inscrever-se na newsletter</label>

<!-- Botão de rádio -->
<input type="radio" name="gender" value="male" id="male">
<label for="male">Masculino</label>
<input type="radio" name="gender" value="female" id="female">
<label for="female">Feminino</label>
```

### 11.2.2 A tag `<textarea>`

Para entrada de texto multilinha, usamos a tag `<textarea>`.

```html
<textarea name="comments" rows="4" cols="50" placeholder="Digite seus comentários aqui"></textarea>
```

### 11.2.3 A tag `<select>`

Para criar listas suspensas, utilizamos a combinação de `<select>` e `<option>`.

```html
<select name="country">
  <option value="">Selecione um país</option>
  <option value="br">Brasil</option>
  <option value="us">Estados Unidos</option>
  <option value="fr">França</option>
</select>
```

## 11.3 Rótulos (Labels)

Os rótulos são importantes para a acessibilidade e usabilidade do formulário.

```html
<label for="email">E-mail:</label>
<input type="email" id="email" name="email" required>
```

## 11.4 Agrupamento de campos

Para organizar melhor os campos do formulário, podemos usar as tags `<fieldset>` e `<legend>`.

```html
<fieldset>
  <legend>Informações Pessoais</legend>
  <label for="name">Nome:</label>
  <input type="text" id="name" name="name" required>
  <label for="email">E-mail:</label>
  <input type="email" id="email" name="email" required>
</fieldset>
```

## 11.5 Botões

Os botões permitem que os usuários enviem o formulário ou realizem outras ações.

```html
<button type="submit">Enviar</button>
<button type="reset">Limpar</button>
<button type="button" onclick="previewForm()">Pré-visualizar</button>
```

## 11.6 Validação de formulários

O HTML5 introduziu atributos de validação incorporados que ajudam a garantir que os dados inseridos sejam válidos antes do envio.

```html
<input type="email" name="email" required>
<input type="number" name="age" min="18" max="100">
<input type="tel" name="phone" pattern="[0-9]{10,11}">
```

## 11.7 Exemplo completo de um formulário

Vamos juntar tudo o que aprendemos em um exemplo completo:

```html
<form action="/submit-registration" method="POST">
  <fieldset>
    <legend>Registro de Usuário</legend>
    
    <label for="username">Nome de usuário:</label>
    <input type="text" id="username" name="username" required>
    
    <label for="email">E-mail:</label>
    <input type="email" id="email" name="email" required>
    
    <label for="password">Senha:</label>
    <input type="password" id="password" name="password" required minlength="8">
    
    <label for="birthdate">Data de nascimento:</label>
    <input type="date" id="birthdate" name="birthdate" required>
    
    <fieldset>
      <legend>Gênero</legend>
      <input type="radio" id="male" name="gender" value="male">
      <label for="male">Masculino</label>
      <input type="radio" id="female" name="gender" value="female">
      <label for="female">Feminino</label>
      <input type="radio" id="other" name="gender" value="other">
      <label for="other">Outro</label>
    </fieldset>
    
    <label for="country">País:</label>
    <select id="country" name="country" required>
      <option value="">Selecione um país</option>
      <option value="br">Brasil</option>
      <option value="us">Estados Unidos</option>
      <option value="fr">França</option>
    </select>
    
    <label for="bio">Biografia:</label>
    <textarea id="bio" name="bio" rows="4" cols="50"></textarea>
    
    <input type="checkbox" id="terms" name="terms" required>
    <label for="terms">Eu aceito os termos e condições</label>
    
    <button type="submit">Registrar</button>
    <button type="reset">Limpar Formulário</button>
  </fieldset>
</form>
```

## Conclusão

Os formulários HTML são uma parte fundamental da interatividade na web. Ao dominar a criação de formulários, você poderá coletar informações dos usuários de maneira eficiente e criar experiências web mais ricas e interativas. Lembre-se sempre de considerar a acessibilidade e a experiência do usuário ao projetar seus formulários.

Este capítulo forneceu uma base sólida para a criação de formulários HTML. À medida que você avança em seu aprendizado de desenvolvimento web, considere explorar técnicas mais avançadas de estilização com CSS e interatividade com JavaScript para criar formulários ainda mais poderosos e atraentes.