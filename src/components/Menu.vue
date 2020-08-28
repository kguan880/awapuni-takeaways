<template>
  <div id="menu" class="container-col">
      <h1>Menu</h1>
    <div class="container-menu">
        <img src="@/assets/menu/packs.jpg" alt="">
        <img src="@/assets/menu/deep-fried.jpg" alt="">
        <img src="@/assets/menu/chinese.jpg" alt="">
        <img src="@/assets/menu/chinese-meal.jpg" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: "Menu",
};
</script>

<style scoped>
h1 {
    text-align: center;
}

.container-menu {
    display:flex;
    width: 95vw;
    height: 80vh;
    align-self: center;
    justify-content: space-between;
}

img{
    height: 100%;
    width: 24%;
}

@media screen and  (max-width: 768px){
  .container-menu{
    flex-direction: column;
    align-items: center;
    height: auto;
  }

  img{
    width: 90%;
    height: 100vh;
  }
}
</style>
