<template>
    <link rel="stylesheet" href="https://unicons.iconscout.com/release/v2.1.9/css/unicons.css">
  <link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/twitter-bootstrap/4.5.0/css/bootstrap.min.css">
<link rel="stylesheet" href="/css/styles.css">
    <div class="login-form">
      <form @submit.prevent="handleLogin">
        <div class="form-group">
          <input type="email" class="form-style" v-model="username" placeholder="Email" required />
          <i class="input-icon uil uil-at"></i>
        </div>
        <div class="form-group mt-2">
          <input type="password" class="form-style" v-model="password" placeholder="Password" required />
          <i class="input-icon uil uil-lock-alt"></i>
        </div>
        <button type="submit" class="btn mt-4">Login</button>
        <p class="mb-0 mt-4 text-center"><a href="#" class="link">Forgot your password?</a></p>
      </form>
    </div>
  </template>
  
  <script>
  export default {
    name: 'LoginForm',
    data() {
      return {
        username: '',
        password: '',
      };
    },
    methods: {
      handleLogin() {
        // Adicione a lógica de login aqui
        console.log('Username:', this.username);
        console.log('Password:', this.password);
      },
    },
  };
  </script>
  
  <style scoped>
  
  </style>
  
