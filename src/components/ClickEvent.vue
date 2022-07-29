<template>
  <div :style="{ background: color }" @click="click">
    clique aqui
  </div>
</template>

<script>
const color = "red";

export default {
  name: "ClickEvent",
  color,
  data() {
    return {
      color
    }
  },
  methods: {
    click() {
      this.color == 'red' ? this.color = 'blue' : this.color = 'red'
    }
  },
}
</script>
