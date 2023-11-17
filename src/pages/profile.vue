<template>
    <div>
      <h3 class="text-2xl font-bold text-left py-2">ACCOUNT CREATION</h3>
      <form @submit.prevent="submitForm">
        <div>
          <label for="username">Username:</label>
          <input type="text" id="username" v-model="username" required />
        </div>
        <div>
          <label for="password">Password:</label>
          <input type="password" id="password" v-model="password" required />
        </div>
        <div>
          <button type="submit">Create Account</button>
        </div>
      </form>
    </div>
  </template>
  
  <script>
  export default 
    {
    data() {
      return {
        username: '',
        password: '',
      };
    },
    methods: {
      submitForm() {
        // Dummy request handling
        console.log('Dummy request submitted:');
        console.log('Username:', this.username);
        console.log('Password:', this.password);
  
      },
    },
  };
  
  </script>
  
  <style>
  
  </style>