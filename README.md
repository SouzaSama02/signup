# 📋 Projeto de Cadastro de Usuários com Vue.js

Bem-vindo(a) ao projeto **Cadastro de Usuários**! Este é um aplicativo simples, mas prático, feito com Vue.js, que permite cadastrar usuários, exibir a lista de cadastros e alternar a visibilidade dessa lista.

> **Tecnologias usadas**: Vue.js 3, HTML, CSS

---

## 🖼️ Visão Geral do Projeto

Este projeto foi desenvolvido para ilustrar como manipular dados de formulário e salvá-los em uma lista (array) em cache, exibindo esses dados após o cadastro. Os usuários podem cadastrar seus dados (nome, idade e e-mail) e exibi-los na tela com um botão que alterna entre exibir e ocultar a lista de usuários cadastrados.

## 🛠️ Funcionalidades

- **Cadastrar Usuários**: Formulário para inserir o nome, idade e e-mail do usuário.
- **Exibir/Ocultar Lista de Cadastros**: Botão para alternar a exibição da lista de usuários cadastrados.
- **Limpeza do Formulário**: Botão para limpar os campos do formulário após o cadastro.

---

## 📂 Estrutura de Pastas

Abaixo está a estrutura básica do projeto para facilitar o entendimento:

```plaintext
📦 cadastro-usuarios
├── 📜 README.md
├── 📂 src
│   ├── 📜 App.vue         # Componente principal
│   ├── 📂 components
│   │   └── 📜 UserForm.vue # Componente de Formulário de Usuários
├── 📂 public
│   └── 📜 index.html
└── 📜 package.json
```

---

## 🚀 Configuração do Ambiente

Siga estas instruções para configurar e executar o projeto localmente:

1. **Clone o repositório**
   ```bash
   git clone https://github.com/seuusuario/cadastro-usuarios.git
   ```
2. **Acesse a pasta do projeto**
   ```bash
   cd cadastro-usuarios
   ```
3. **Instale as dependências**
   ```bash
   npm install
   ```
4. **Execute o projeto**
   ```bash
   npm run serve
   ```

O projeto estará disponível em [http://localhost:8080](http://localhost:8080).

---

## 📝 Como Funciona

### 1. Formulário de Cadastro

- **Nome**: Campo obrigatório, tipo `text`.
- **Idade**: Campo obrigatório, tipo `number` com limite de 150.
- **E-mail**: Campo obrigatório, tipo `email`.

### 2. Botão de Exibir/Ocultar Lista

O botão “Exibir/Ocultar Informações” alterna a visibilidade da lista de usuários cadastrados. Quando a lista está visível, o texto do botão exibe "Ocultar Informações", e quando está oculta, o texto exibe "Exibir Informações".

### 3. Armazenamento em Array

Cada usuário cadastrado é armazenado em uma array chamada `users`. Essa array é exibida em uma lista no HTML, onde cada item é o cadastro de um usuário.

---

## 🎯 Exemplos de Uso

1. **Cadastro de um Usuário**

   - Preencha o formulário com um nome, idade e e-mail.
   - Clique em "Cadastrar".
   - O cadastro será salvo e aparecerá na lista abaixo (caso a lista esteja visível).

2. **Exibir/Ocultar Lista**
   - Clique no botão "Exibir Informações" para mostrar a lista.
   - Clique em "Ocultar Informações" para escondê-la.

---

## 🖌️ Estilização

Abaixo estão alguns estilos simples aplicados ao botão e à lista para tornar a interface amigável:

```css
button {
  margin-top: 1em;
  padding: 0.5em 1em;
  background-color: #4caf50; /* Verde para o botão de cadastro */
  color: white;
  border: none;
  cursor: pointer;
}

button:hover {
  background-color: #45a049;
}

li span {
  margin-right: 1em;
  font-weight: bold;
}
```

---

## 🤔 Possíveis Melhorias

- **Validação Avançada**: Implementar validações mais complexas, como idade mínima e formatos de e-mail mais estritos.
- **Persistência de Dados**: Armazenar os dados localmente (ex.: `localStorage`) para manter os cadastros mesmo após o fechamento do navegador.
- **Componentização**: Dividir o formulário e a lista em componentes separados para maior modularidade.

---

## 🤝 Contribuições

Contribuições são bem-vindas! Sinta-se à vontade para abrir um _issue_ ou _pull request_ para adicionar uma melhoria ou corrigir um problema.

---

## 🧑‍💻 Autor

Desenvolvido por [Lucas](https://www.linkedin.com/in/seulinkedin). Se gostou do projeto, deixe uma ⭐ e compartilhe com outros desenvolvedores!

---

## 📜 Licença

Distribuído sob a licença MIT. Veja `LICENSE` para mais informações.

---

Obrigado por conferir o projeto! 💚

```

Esse `README.md` apresenta todas as informações relevantes sobre o projeto, incluindo instruções para configuração, funcionamento e possíveis melhorias. Sinta-se à vontade para adaptá-lo conforme necessário, incluindo links para capturas de tela ou GIFs que demonstrem a interface do projeto em funcionamento!
```
