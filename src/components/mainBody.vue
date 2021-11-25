<template>
<div id="page">
    <div id="container">
        <SubMain/>
    </div>
</div>
</template>

<script>
import SubMain from '../components/SubMain.vue';

export default {
  name: 'MainBody',
  components: {
      SubMain,
  },
  
}
</script>
<style scoped lang="scss">
#page {
    background-color: rgb(47, 47, 47);
    /* debug */
    height: 150px;
}
#container {
    width: 70%;
    margin: auto;
    color: white;
}
</style>
