<template>
  <div>
    <p v-if="esta_trabalhando">Estou trabalhando no momento.</p>
    <p v-else>Estou em busca de oportunidade</p>
    <p v-if="4 > 6">Testando</p>
    <p>Utilizo as seguintes tecnologias</p>
    <ul>
      <li>JavaScript</li>
      <li>PHP</li>
      <li>Python</li>
    </ul>
    <button @click="showEmail">{{textoBotao}}</button>
    <p v-show="mostrar_email">Mande uma mensagem para {{ email }}</p>
    <p class="teste">
      Para acessar meu portifolio
      <a v-bind:href="meu_link" target="_blank"> basta clicar aqui</a>
    </p>
    <Picture />
  </div>
</template>
<script>
import Picture from "./form/Picture.vue";
export default {
  name: "Info",
  components: {
    Picture,
  },
  data() {
    return {
      esta_trabalhando: false,
      mostrar_email: false,
      email: "edson@edson.com",
      meu_link: "https://www.google.com/",
      textoBotao : "Mostrar email"
    };
  },
  methods:{
    showEmail(){
      this.mostrar_email =!this.mostrar_email
      if(!this.mostrar_email){
        this.textoBotao = "Mostrar email"
      }else{
        this.textoBotao = "Esconder email"
      }
    }
  }
};
</script>
<style>
.paragrafo-pai{
  color: red;
}
</style>