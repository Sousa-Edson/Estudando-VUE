<template>
  <img :src="avatar" :alt="descricao" />
</template>

<script>
export default {
  name: "Picture",
  data() {
    return {
      avatar: "/img/avatar.png",
      descricao: "nome da imagem",
    };
  },
};
</script>

<style>
</style>