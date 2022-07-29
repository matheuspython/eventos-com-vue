<template>
  <main>
    <h1 class="title">escolha o evento</h1>
    <div class="container">
      <ClickEvent class="box" />
      <HoverEvent class="box" />
    </div>
  </main>
</template>

<script>
import ClickEvent from './ClickEvent.vue';
import HoverEvent from './HoverEvent.vue';
export default {
  name: "TheMain",
  components: { ClickEvent, HoverEvent }
}
</script>

<style scoped>
.box {
  width: 100%;
  max-width: 300px;
  height: 85px;
  color: #ffff;
  display: flex;
  align-items: center;
  justify-content: center;
  border-radius: 15px;
}

.title {
  text-align: center;
  margin: 20px 0;
}

.container {
  width: 100%;
  max-width: 1280px;
  gap: 15px;
  margin: 0 auto;
  text-transform: uppercase;
  display: flex;
  justify-content: center;
  align-items: center;
}
</style>