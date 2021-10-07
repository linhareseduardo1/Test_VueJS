<template>
  <div class="hello">
    <h1>Revisão do cadastro</h1>
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
        <label for="name">Nome completo </label>
        <br />
        <span> {{ name }}</span>
      </p>

      <p>
        <label for="age">CPF </label><br />
        <span> {{ cpf }}</span>
      </p>

      <p>
        <label for="age">Número de celular </label><br />
        <span> {{ phone }}</span>
      </p>

      <p>
        <label for="estado">Estado/Cidade </label><br />
        <span> {{ estado }}</span>
        <span> {{ cidade }}</span>
      </p>
      <p>
        <label for="especialidade">Especialidade Principal </label><br />
        <span> {{ especialidade }}</span>
      </p>

      <p>
        <label for="preco"> Preço da consulta </label><br />
        <span> {{ preco }}</span>
      </p>

      <p>
        <label for="pag"> Forma de pagamento da consulta </label><br />
        <span> {{ pag }}</span>
      </p>

      <p>
        <input type="submit" value="CADASTRAR" />
      </p>
    </form>
  </div>
</template>

<script>
export default { name: "PageRevisao" };
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
