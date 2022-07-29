<template>
  <div>
    <form action="https://google.com" @submit.prevent="onSubmit">
      <input v-model="nameOfPeople" placeholder="escreva seu nome aqui" @keyup.enter="onKeyUp" type="text">

      <button type="submit">Enviar</button>
      {{nameOfPeople}}
    </form>
  </div>
</template>


<script>
export default {
  name: 'FormEvent',
  data(){
    return{
      nameOfPeople: this.nameOfPeople
    }
  },  
  methods: {
    onKeyUp() {
      alert('Olá seja bem vindo ',this.nameOfPeople)
    },
      onSubmit() {
        alert('seja bem vindo '+this.nameOfPeople)
      }
  },
}
</script>

<style scoped>
div {
  background-color: rgb(103, 108, 227);
}

form {
  gap: 15px;
  display: flex;
  flex-direction: column;
}

input {
  height: 35px;
  padding-left: 15px;
  border-radius: 12px;
  border: none;
  background-color: rgb(81, 86, 219);
  color: #fff;


  width: 100%;
}
input::placeholder {
  color: #fff;
}
button{
  border: 0;
  height: 25px;
  background-color: #1830e9;
  color: #fff;
  cursor: pointer;
  border-radius: 8px;
  transition: .4s;
}
button:hover{
   background-color: #5666e2;
}
</style>