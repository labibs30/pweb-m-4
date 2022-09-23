<template>
  <h1>{{title}}</h1>
  <Modal :header="header" :text="text"/>
</template>

<script>
import HelloWorld from './components/HelloWorld.vue'
import Modal from './components/Modal.vue'
export default {
  name: 'App',
  components: {
    HelloWorld, Modal
  },
  data(){
    return{
      title:'Vue App',
      header:'Mobil',
      text:'Motor'
    }
  },
  methods:{
    handleClick(){
      this.$refs.name1.classList.add('active');
      this.$refs.name1.focus();
      console.log(this.$refs.name1);
  }
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  margin-top: 60px;
}
</style>
