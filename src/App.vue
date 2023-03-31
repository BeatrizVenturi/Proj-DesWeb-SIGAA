<script setup>
import { ref } from "vue"
const nome = ''
const Email = ''
const Senha = ''
const SenhaConfirmar = ''

</script>

<template>
  <h1>Ediçao De Perfil</h1>
  <div>
    Diga seu nome <input type="text" v-model="nome" placeholder="Nome" required />
  </div>
  <div>
    Diga seu e-mail <input type="text" v-model="email" placeholder="Email" required />
  </div>
  <div>
    Diga sua senha <input type="text" v-model="Senha" placeholder="Senha" required />
  </div>
  <div>
    Confirme sua senha <input type="text" v-model="SenhaConfirmar" placeholder="Confirmar senha" required />
  </div>
  

  
</template>

<style scoped></style>
