<template>
  <div class="box">
      <div class="comics">
        <img :src="dcBook.thumb" :alt="dcBook.series">
      </div>
      <h3>
        {{dcBook.series}}
      </h3>
      <span>
        {{dcBook.type}}
        <br>
        {{dcBook.price}}
      </span>
  </div>
</template>

<script>
export default {
  name: 'SubMain',
  props: {
    dcBook: Object,
  }
}
</script>
<style scoped lang="scss">
.box{
  width: calc((100% / 6) - 20px);
  margin: 10px;
  /* debug */
  /* height: 100px; */
  /* background-color: red; */
  /* border: 1px solid white; */

  .comics {
    width: 100%;
    /* debug */
    /* height: 80%;
    background-color: black; */

    img{
      width: 100%;
    }
  }

  h3 {
    color: white;
  }
}
</style>
