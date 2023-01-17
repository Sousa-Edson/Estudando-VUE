<template>
  <div>
    <h2>Meu formulario</h2>
    <form action="">
      <div>
        <InputTexto />
      </div>
      <div>
        <InputTexto />
      </div>

      <Submit />
    </form>
  </div>
</template>
<script>
import Submit from "./form/Submit.vue";
import InputTexto from "./form/InputTexto.vue";
export default {
  name: "Formulario",
  components: {
    Submit,
    InputTexto,
  },
};
</script>