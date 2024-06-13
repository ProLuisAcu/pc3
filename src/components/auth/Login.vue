<template>
  <div class="login">
    <h1>Login</h1>
    <form @submit.prevent="handleSubmit">
      <input v-model="username" type="text" placeholder="Username" required />
      <input
        v-model="password"
        type="password"
        placeholder="Password"
        required
      />
      <button type="submit" class="btn btn-primary btn-block btn-large">
        Ingresar
      </button>
      <p v-if="error" class="error-message">{{ error }}</p>
    </form>
  </div>
</template>
