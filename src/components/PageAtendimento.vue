<template>
  <div class="hello">
    <div
      class="vue-bg col-md-5 h100 d-flex justify-content-center align-items-center"
    >
      <img alt="Vue logo" src="../assets/logo.png" width="25%" />
    </div>
    <div
      class="col-md-9 h-100 d-flex justify-content-center align-items-center"
    >
      <div class="col-md-5 rounded px-5 py-4 shadow bg-white text-left">
        <h1>Sobre o atendimento</h1>
        <h2>Dados do atendimento</h2>
        <div id="header"></div>
        <form id="home" @submit="checkForm" action="#" method="post">
          <!--
  <p v-if="errors.length">
    <b>Por favor, corrija o(s) seguinte(s) erro(s):</b>
    <ul>
      <li v-for="error in errors">{{ error }}</li>
    </ul>
  </p> -->
          <p>
            <label for="name">Especialidade principal* </label>
            <br />

            <select v-model="selected">
              <option disabled value="">Escolha um item</option>
              <option>Cardiologia</option>
              <option>Dermatologia</option>
              <option>Neurologia</option>
              <option>Oftalmologia</option>
              <option>Psiquiatria</option>
              <option>Urologia</option>
            </select>
            <br />
          </p>

          <p>
            <label for="preco">Informe o preço da consulta* </label><br />
            <input
              id="money"
              v-model="money"
              type="money"
              name="cpf"
              min="9"
              max="9"
              placeholder="R$ 00,00"
            />
          </p>

          <p>
            <label for="Pag">Forma de Pagamento* </label><br />

            Pix:
            <input
              type="checkbox"
              v-model="toggle"
              true-value="sim"
              false-value="não"
            /><br />
            Em dinheiro:
            <input
              type="checkbox"
              v-model="toggle"
              true-value="sim"
              false-value="não"
            />
            <br />
            Cartão de crédito:
            <input
              type="checkbox"
              v-model="toggle"
              true-value="sim"
              false-value="não"
            /><br />
          </p>
          <p>
            <input type="submit" value="PRÓXIMO" />
          </p>
        </form>
      </div>
    </div>
  </div>
</template>


<script>
export default { name: "PageAtendimento" };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
a {
  color: #42b983;
}
</style>
