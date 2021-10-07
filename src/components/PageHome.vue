<template>
  <div class="hello">
    <h1>Sobre o profissional</h1>
    <h2>Dados do profissional</h2>
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
        <label for="name">Nome completo* </label>
        <br />
        <input
          id="name"
          v-model="name"
          type="text"
          name="name"
          placeholder="Digite o nome completo"
        />
      </p>

      <p>
        <label for="age">CPF* </label><br />
        <input
          id="cpf"
          v-model="cpf"
          type="cpf"
          name="cpf"
          min="9"
          max="9"
          placeholder="Digite um CPF"
        />
      </p>

      <p>
        <label for="tel">Número de celular* </label><br />
        <input
          id="tel"
          v-model="phone"
          type="cpf"
          name="cpf"
          min="9"
          max="9"
          placeholder="(00) 0 0000-0000"
        />
      </p>
      <p>
        <label for="estado">Estado* </label><br />
        <select id="estado" v-model="estado" name="estado">
          <option>Paraná</option>
          <option>Rio Grande do Sul</option>
          <option>Santa Catarina</option>
        </select>
      </p>
      <p>
        <label for="cidade">Cidade* </label><br />
        <select id="cidade" v-model="cidade" name="estado">
          <option>Londrina(PR)</option>
          <option>Maringá(PR)</option>
          <option>Pelotas(RS)</option>
          <option>Porto Alegre(RS)</option>
          <option>Florianópolis(SC)</option>
          <option>Joinville (RS-)</option>
        </select>
      </p>
      <p>
        <input type="submit" value="PRÓXIMO" />
      </p>
    </form>
  </div>
</template>

<script>
export default { name: "PageHome" };
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style lang="scss">
$primary-0: #483698;

h1 {
  color: $primary-0;
  font-family: Verdana, Geneva, Tahoma, sans-serif;
}
</style>


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
