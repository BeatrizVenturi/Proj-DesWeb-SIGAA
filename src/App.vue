<script setup>
import { ref } from "vue"
const nome = ''
const Email = ''
const Senha = ''
const SenhaConfirmar = ''

const anoNascimento = ''
const dia = ''
const Cidade = ''
const mes = ''
const estado = ''
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







  <div class="mb-3">
    Estado
    <select class="form-select" v-model="estado" required aria-label="select example">
      <option value="">Estado </option>
      <option value="Acre">AC</option>
      <option value="Alagoas">AL</option>
      <option value="Amapa">AP</option>
      <option value="Bahia">BA</option>
      <option value="Ceara">CE</option>
      <option value="DistritoFederal">DF</option>
      <option value="EspiritoSanto">ES</option>
      <option value="Goiania">GO</option>
      <option value="Maranhao">MA</option>
      <option value="MatoGrosso">MT</option>
      <option value="MatoGrossoDoSul">MS</option>
      <option value="MinasGerais">MG</option>
      <option value="Para">PA</option>
      <option value="Paraiba">PB</option>
      <option value="Parana">PR</option>
      <option value="Pernambuco">PE</option>
      <option value="Piaui">PI</option>
      <option value="RioDeJaneiro">RJ</option>
      <option value="RioGrandeDoNorte">RN</option>
      <option value="RioGrandeDoSul">RS</option>
      <option value="Rondonia">RO</option>
      <option value="Roraima">RR</option>
      <option value="SantaCatarina">SC</option>
      <option value="SaoPaulo">SP</option>
      <option value="Sergipe">SE</option>
      <option value="Tocantins">TO</option>
     
    </select>
  </div>

  
</template>

<style scoped></style>


