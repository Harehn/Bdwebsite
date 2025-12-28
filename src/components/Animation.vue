<template>
  <div class="animation">
    <div class="wrapper">
        <img id="top" :src="require(`@/assets/present_top.png`)" alt="">
        <img id="bottom" :src="require(`@/assets/present_bottom.png`)" alt="">
    </div>
  </div>
</template>

<script>
export default {
  name: 'Animation',
  props: {
    message: String
  }
  
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.wrapper {
    height:40%;
    width:40%;
    margin:auto;
    opacity:0.6;
}
.animation {
    height:100%;
    width:100%;
    color:white;
    /* font-family: monospace; */
    text-align: center;
    align-content: center;
    /* background-color: crimson; */
    background-image: url('~@/assets/present.jpg');
}
#top {
    /* opacity:0.6; */
    height:50%;
}
#bottom {
    height:52%;
}
</style>
