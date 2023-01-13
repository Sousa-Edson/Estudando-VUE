<template>
  <div>
    <h1>Ola vue</h1>
    <p>Meu nome é {{ nome }} e trabalho com {{ profissao }}</p>
  </div>
</template>
<script>
export default {
  name: "PrimeiroComponente",
  data() {
    return {
      nome: "Edson",
      profissao:"programador"
    };
  },
};
</script>
