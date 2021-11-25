<template>
  <div id="container">
      <!-- logo -->
      <span>
        <img src="../assets/img/dc-logo.png" alt="logo DC">
      </span>
      <!-- nav menu -->
      <nav>
          <!-- menu -->
          <ul>
              <li v-for="point, i in navList" :key="i">
                  <a :href="point.url" :class="point.active == true ? `selected` : ``">{{point.text}}</a>
              </li>
              <!-- 10 -->
          </ul>
      </nav>
  </div>
</template>

<script>
export default {
  name: 'Header',
  data() {
      return {
          navList :[
              {
                text:"CHARACTERS",
                url:"#",
                active: false
              },
              {
                text:"COMICS",
                url:"#",
                active: true
              },
              {
                text:"MOVIE",
                url:"#",
                active: false
              },
              {
                text:"TV",
                url:"#",
                active: false
              },
              {
                text:"GAMES",
                url:"#",
                active: false
              },
              {
                text:"COLLECTIBLES",
                url:"#",
                active: false
              },
              {
                text:"VIDEOS",
                url:"#",
                active: false
              },
              {
                text:"FANS",
                url:"#",
                active: false
              },
              {
                text:"NESW",
                url:"#",
                active: false
              },
              {
                text:"SHOP",
                url:"#",
                active: false
              },
              
          ]
      }
  }
}
</script>

<style scoped lang="scss">
#container {
    width: 70%;
    margin: 10px auto;
    display: flex;
    align-items: center;
    justify-content: space-between;
}
li {
    display: inline-block;
    margin: 0 10px;
}

a {
    color: black;
    text-decoration: none;
}

.selected {
  color: blue;
  padding-bottom: 50px;
  border-bottom: 5px solid blue;
}
</style>
