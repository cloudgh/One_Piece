<template>
  <div class="header">
      <button  @click="goTo('/')">О сериале</button>
      <button  @click="goTo('/page2')">Трейлер</button>
      <button  @click="goTo('/page3')">Галерея</button>
  </div>
</template>
<script>
export default {
    methods: {
      goTo(route) {
        this.$router.push(route);
      } 
    }
  }
</script>

<style lang="scss" scoped>
.header {
  color: black;
  display: flex;
  justify-content: center;
  button {
    width: 200px;
    background-color: rgba(231, 214, 182, 0.747);
    border-radius: 8px;
    border: 2px solid  rgb(158, 113, 113);
    padding: 10px 20px;
    font-size: 18px;
    font-weight: bold;
    cursor: pointer;
    text-decoration: none;
    margin: 10px;
  }
  button:hover {
    transform: translateY(-5px);
    transition: transform 0.1s ease-out;
  }
}
</style>