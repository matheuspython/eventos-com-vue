<template>
  <div 
    :style="{ background: cor }"
    @mouseover="onMouseOver"
    @mouseout="onMouseOut"
  >
    {{text}}
  </div>
</template>

<script>  
  const cor = "#5d25be"
  export default {
    name: "HoverEvent",
    text: 'coloque o mouse aqui',
    cor,
    data(){
      return{
         text: 'coloque o mouse aqui',
         cor
      }
    },
    methods: {
      onMouseOver(){
        this.text = 'tire o mouse aqui'
        this.cor = 'blue'
      },
      onMouseOut(){
        this.text ='coloque o mouse aqui'
        this.cor = '#5d25be'

      }
    },
  }
</script>
