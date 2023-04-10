<script setup>
import { ref } from "vue"

const nome = ref('')
const Email = ref('')
const Senha = ref('')
const SenhaConfirmar = ref('')
const dia = ref('')
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
      <h1>Ediçao De Perfil</h1>
      <div>
        Diga seu nome <input type="text" v-model="nome" placeholder="Nome" required />
      </div>
      <div>
        Diga seu e-mail <input type="email" v-model="Email" placeholder="Email" required />
      </div>
      <div>
        Diga sua senha <input type="text" v-model="Senha" placeholder="Senha" required />
      </div>
      <div>
        Confirme sua senha <input type="text" v-model="SenhaConfirmar" placeholder="Confirmar senha" required />
      </div>



      <div class="mb-3">
        Data Nascimento:
        <select class="form-select" v-model="dia" required aria-label="select example">
          <option value="">Dia </option>
          <option value="1">1</option>
          <option value="2">2</option>
          <option value="3">3</option>
          <option value="4">4</option>
          <option value="5">5</option>
          <option value="6">6</option>
          <option value="7">7</option>
          <option value="8">8</option>
          <option value="9">9</option>
          <option value="10">10</option>
          <option value="11">11</option>
          <option value="12">12</option>
          <option value="13">13</option>
          <option value="14">14</option>
          <option value="15">15</option>
          <option value="16">16</option>
          <option value="17">17</option>
          <option value="18">18</option>
          <option value="19">19</option>
          <option value="20">20</option>
          <option value="21">21</option>
          <option value="22">22</option>
          <option value="23">23</option>
          <option value="24">24</option>
          <option value="25">25</option>
          <option value="26">26</option>
          <option value="27">27</option>
          <option value="28">28</option>
          <option value="29">29</option>
          <option value="30">30</option>
          <option value="31">31</option>
        </select>

        <input type="month" v-model="mes">
      </div>

      <div>
        Diga sua ciadade <input type="text" v-model="Cidade" placeholder="Diga sua cidade" required />
      </div>

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

      <div>
        Hobbies: <input type="text" v-model="Hobbie" placeholder="Hobbies" required />
      </div>


      <div class="mb-3">
        Data Nascimento:
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

        <div>Diga uma biografia curta:</div>
        <div>
          <textarea class="form-control" v-model="biografia" id="validationTextarea"
            placeholder="Digite Aqui Sua Biografia" required></textarea>
        </div>


        <div> <button type="submit" class="btn btn-outline-primary"> Enviar </button> </div>


        <div v-if="mostrar">

          <div> <strong> Nome: </strong> {{ nome }}</div>
          <div> <strong> Email:</strong> {{ Email }}</div>
          <div> <strong> Senha: </strong> {{ SenhaConfirmar }}</div>
          <div> <strong> Data Nascimento: dia</strong> {{ dia }} <strong>de</strong> {{ mes }}</div>
          <div> <strong> Cidade: </strong>{{ Cidade }}</div>
          <div> <strong> Estado:</strong> {{ estado }}</div>
          <div> <strong> Hobbies:</strong> {{ Hobbie }}</div>
          <div> <strong> Linguagem de Programação:</strong> {{ LinguagemProg }}</div>
          <div> <strong> Biografia:</strong> {{ biografia }} </div>


        </div>

    </form>

  </div>
</template>


<style scoped>
.editor {
  background-color: aquamarine;



}
</style>


