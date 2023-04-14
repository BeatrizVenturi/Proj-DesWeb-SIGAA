<script setup>
import { ref } from "vue"

const nome = ref('')
const Email = ref('')
const Senha = ref('')
const SenhaConfirmar = ref('')
const mes = ref('')
const Cidade = ref('')
const estado = ref('')
const Hobbie = ref('')
const LinguagemProg = ref('')
const biografia = ref('')
const mostrar = ref(false)
</script>

<template>
  <div class="editor">

    <form @submit.prevent="mostrar = !mostrar">
      <div class="titulo">
        <h1>Ediçao De Perfil</h1>
      </div>


      <div>
        Diga seu nome: <br>
        <input type="text" v-model="nome" placeholder="Nome" required />
      </div>
      <div>
        Diga seu e-mail: <br> <input type="email" v-model="Email" placeholder="Email" required />
      </div>
      <div>
        Diga sua senha: <br> <input type="text" v-model="Senha" placeholder="Senha" required />
      </div>
      <div>
        Confirme sua senha: <br> <input type="text" v-model="SenhaConfirmar" placeholder="Confirmar senha" required />
      </div>
      Sua data de Nascimento: <br> <input type="date" v-model="mes">
      <div>
        Diga sua ciadade <br> <input type="text" v-model="Cidade" placeholder="Diga sua cidade" required />
      </div>


      <div class="sla">
        <div class="mb-3">
          Estado:
          <select class="form-select" v-model="estado" required aria-label="select example">
            <option value="">Estado </option>
            <option value="Acre">AC</option>
            <option value="Alagoas">AL</option>
            <option value="Amapá">AP</option>
            <option value="Bahia">BA</option>
            <option value="Ceará">CE</option>
            <option value="Distrito Federal">DF</option>
            <option value="Espirito Santo">ES</option>
            <option value="Goiania">GO</option>
            <option value="Maranhão">MA</option>
            <option value="Mato Grosso">MT</option>
            <option value="Mato Grosso Do Sul">MS</option>
            <option value="Minas Gerais">MG</option>
            <option value="Pará">PA</option>
            <option value="Paraiba">PB</option>
            <option value="Parana">PR</option>
            <option value="Pernambuco">PE</option>
            <option value="Piauí">PI</option>
            <option value="Rio De Janeiro">RJ</option>
            <option value="Rio Grande Do Norte">RN</option>
            <option value="Rio Grande Do Sul">RS</option>
            <option value="Rondonia">RO</option>
            <option value="Roraima">RR</option>
            <option value="SantaC atarina">SC</option>
            <option value="São Paulo">SP</option>
            <option value="Sergipe">SE</option>
            <option value="Tocantins">TO</option>
          </select>
        </div>
      </div>

      <div>
        Hobbies: <br>
        <input type="text" v-model="Hobbie" placeholder="Hobbies" required />
      </div>


      <div class="mb-3">
        Linguagem de Programação:
        <div class="sla">
          <select class="form-select" v-model="LinguagemProg" required aria-label="select example">
            <option selected disabled value="">Selecione</option>
            <option value="JS">JS</option>
            <option value="Java">Java</option>
            <option value="JavaScript">JavaScript</option>
            <option value="C++">C++</option>
            <option value="PHP">PHP</option>
            <option value="C#">C#</option>
            <option value="TypeScript">TypeScript</option>
            <option value="Ruby">Ruby</option>
            <option value="VueJs">Vue.js</option>
            <option value="C">C</option>
            <option value="Swift">Swift</option>
          </select>
        </div>
      </div>
      <div>Diga uma biografia curta:</div>
      <div>
        <div class="bio"> <textarea class="form-control" v-model="biografia" id="validationTextarea"
            placeholder="Digite Aqui Sua Biografia" required></textarea>
        </div>
      </div>





      <div class="titulo ">

        <div> <button type="submit" class="btn btn-outline-light"> Enviar </button> </div>
      </div>
      <div class="Final">
        <div v-if="mostrar">
          <h1>Perfil Atualizado</h1>
          <div> <strong> Nome: </strong> {{ nome }}</div>
          <div> <strong> Email:</strong> {{ Email }}</div>
          <div> <strong> Senha: </strong> {{ SenhaConfirmar }}</div>
          <div> <strong> Data Nascimento:</strong> {{ mes }}</div>
          <div> <strong> Cidade: </strong>{{ Cidade }}</div>
          <div> <strong> Estado:</strong> {{ estado }}</div>
          <div> <strong> Hobbies:</strong> {{ Hobbie }}</div>
          <div> <strong> Linguagem de Programação:</strong> {{ LinguagemProg }}</div>
          <div> <strong> Biografia:</strong> {{ biografia }} </div>

        </div>
      </div>
    </form>

  </div>
</template>


<style scoped>
.editor {
  margin-right: 650px;
  margin-left: 650px;
  margin-top: 30px;
  margin-bottom: 30px;
  padding-bottom: 10px;
  border-radius: 10px;
  padding-left: 5px;
  color: white;
  padding-left: 20px;
  padding-right: 20px;
  background-color: brown;

}

.titulo {
  text-align: center;
  padding-top: 10px;
}

.sla {
  padding-right: 330px;
}

.bio {
  padding-right: 40px;
}

</style>


