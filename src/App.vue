<template>
  <div id="app" class="">
    <PageAtendimento />
  </div>
</template>


<script>
import PageAtendimento from "./components/PageAtendimento.vue";

export default {
  components: {
    PageAtendimento: PageAtendimento,
  },
};
</script>
<!--
<script>
import PageHome from "./components/PageHome.vue";

export default {
  components: {
    PageHome: PageHome,
  },
};
</script>


<script>
import PageRevisao from "./components/PageRevisao.vue";

export default {
  components: {
    PageHome: PageRevisao,
  },
};
</script>

-->

<style lang="scss">
$primary-0: #483698;
$secondary-0: #ffffff;
$secondary-1: #f9f9f9;
$secondary-3: #b9b9b9;
$secondary-4: #8a8a8a;
$secondary-7: #282828;
$cta-1: #ffe766;
$cta-0: #fbde40;
$danger: #dc3545; //
$transparent: none;
@import url("https://fonts.googleapis.com/css2?family=Comfortaa:wght@300&display=swap");

h1 {
  color: $primary-0;
  font-family: "Comfortaa", cursive;
}
h2,
h3,
h4 {
  color: $primary-0;
  font-family: "Open Sans";
}
</style>

<style>
#app {
  font-family: "Confortaa";
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: left;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
