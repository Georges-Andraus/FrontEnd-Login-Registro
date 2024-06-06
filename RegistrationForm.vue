<template>
     <link rel="stylesheet" href="https://unicons.iconscout.com/release/v2.1.9/css/unicons.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.5.0/css/bootstrap.min.css">
<link rel="stylesheet" href="/css/styles.css">
    <div class="registration-form">
      <form @submit.prevent="handleCadastro">
        <div class="form-group">
          <input type="text" class="form-style" v-model="username" placeholder="Full Name" required />
          <i class="input-icon uil uil-user"></i>
        </div>
      <div class="form-group mt-2">
        <input type="email" class="form-style" v-model="email" placeholder="Email" required />
        <i class="input-icon uil uil-at"></i>
      </div>
      <div class="form-group mt-2">
        <input type="password" class="form-style" v-model="password" placeholder="Password" required />
        <i class="input-icon uil uil-lock-alt"></i>
      </div>
      <button type="submit" class="btn mt-4">Register</button>
    </form>
  </div>
</template>

<script>
export default {
  name: 'RegistrationForm',
  data() {
    return {
      username: '',
      phone: '',
      email: '',
      password: '',
    };
  },
  methods: {
    handleCadastro() {
      // Adicione a lógica de cadastro aqui
      console.log('Username:', this.username);
      console.log('Email:', this.email);
      console.log('Password:', this.password);
    },
  },
};
</script>

<style scoped>

</style>

  
