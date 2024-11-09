<script>
export default {
  data() {
    return {
      showContent: false,
      user: {
        name: "",
        years: "",
        mail: "",
      },
      users: [],
    };
  },
  methods: {
    registerUser() {
      this.users.push({ ...this.user });
      this.clearForm();
    },
    clearForm() {
      this.user.name = "";
      this.user.years = "";
      this.user.mail = "";
    },
    toggleContent() {
      this.showContent = !this.showContent;
    },
  },
};
</script>

<template>
  <div>
    <div>
      <h2>Lista de Cadastros</h2>
      <button class="exibir" @click="toggleContent">
        {{ showContent ? "Ocultar" : "Exibir" }} Informações
      </button>
      <ul v-show="showContent">
        <li v-for="(user, index) in users" :key="index">
          <span>Nome: {{ user.name }}</span>
          <span>Idade: {{ user.years }} anos</span>
          <span>Email: {{ user.mail }}</span>
        </li>
      </ul>
    </div>

    <!-- Formulário de cadastro -->
    <form @submit.prevent="registerUser">
      <div>
        <label for="name">Nome:</label>
        <input
          required
          placeholder="Ex: Lucas"
          type="text"
          id="name"
          name="name"
          v-model="user.name"
        />
      </div>
      <div>
        <label for="years">Idade:</label>
        <input
          required
          placeholder="Ex: 19"
          type="number"
          name="years"
          id="years"
          max="150"
          v-model="user.years"
        />
      </div>
      <div>
        <label for="mail">Email:</label>
        <input
          required
          placeholder="Ex: lucas@exemplo.com"
          type="email"
          name="mail"
          id="mail"
          v-model="user.mail"
        />
      </div>
      <button type="submit">Cadastrar</button>
      <button type="reset" @click="clearForm">Limpar Campos</button>
    </form>
  </div>
</template>

<style scoped>
button {
  margin-top: 1em;
}

li span {
  margin-right: 1em;
}
.exibir {
  margin-bottom: 1em;
}
</style>
