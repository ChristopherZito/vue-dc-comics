<template>
  <div id="foot-page">
        <!-- shop -->
        <div id="shop">
            <!-- <section>
                <ul>
                    <li v-for="product,i in shopSection" :key="i">
                        <img :src="require(`./assets/img/${product.img}`)" :alt="product.text">
                        <h3>
                            {{product.text}}
                        </h3>
                    </li>
                </ul>
            </section> -->
        </div>
        <!-- footer links -->
        <div id="foot-link">
            <section>
                <div id="for-flex">
                    <!-- array 1/4 & 2/4 -->
                    <div>
                        <div >
                            <h1>
                                DC COMICS
                            </h1>
                            <ul>
                                <li v-for="link,i in dcComics" :key="i">
                                    <a :href="link.url">
                                        {{link.text}} 
                                    </a>
                                </li>
                            </ul>
                        </div>
                        <div >
                            <h1>
                                SHOP
                            </h1>
                            <ul>
                                <li v-for="link,i in shop" :key="i">
                                    <a :href="link.url">
                                        {{link.text}}
                                    </a>
                                </li>
                            </ul>
                        </div>
                    </div>
                    <!-- array 3/4 -->
                    <div >
                        <h1>
                            DC
                        </h1>
                        <ul>
                            <li v-for="link,i in dc" :key="i">
                                <a :href="link.url">
                                    {{link.text}}
                                </a>
                            </li>
                        </ul>
                    </div>
                    <!-- array 4/4 -->
                    <div >
                        <h1>
                            SITES
                        </h1>
                        <ul>
                            <li v-for="link,i in sites" :key="i">
                                <a :href="link.url">
                                    {{link.text}}
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
                <figure>
                    <img src="../assets/img/dc-logo-bg.png" alt="">
                </figure>
            </section>
      </div>
      <!-- sing-up -->
      <div id="sing-up">
          <div id="bottom-page">
              <!-- sing-up -->
              <button>
                  <h2>
                      SING-UP NOW!
                  </h2>
              </button>
              <!-- social -->
              <div>
                  <h2>
                      FOLLOW US
                  </h2>
                  <img src="../assets/img/footer-facebook.png" alt="">
                  <img src="../assets/img/footer-periscope.png" alt="">
                  <img src="../assets/img/footer-pinterest.png" alt="">
                  <img src="../assets/img/footer-twitter.png" alt="">
                  <img src="../assets/img/footer-youtube.png" alt="">

              </div>
          </div>
      </div>
  </div>
</template>

<script>
export default {
  name: 'FootPage',
  data() {
      return {
          /* parte blu del footer */
          shopSection: [
              {
                img:"buy-comics-digital-comics.png",
                text:"DIGITAL COMICS",
              },
              {
                img:"buy-comics-merchandise.png",
                text:"DC MERCHANDISE",
              },
              {
                img:"buy-comics-subscriptions.png",
                text:"SUBSCRIPTION",
              },
              {
                img:"buy-comics-shop-locator.png",
                text:"COMIC SHOP LOCATOR",
              },
              {
                img:"buy-dc-power-visa.svg",
                text:"DC POWER VISA",
              },
          ],
          /* parte centrale del footer */
          /* array 1/4 */
          dcComics:[
            {
                text:"Characters",
                url:"#",
            }, 
            {
                text:"Comics",
                url:"#"
            },   
            {
                text:"movies",
                url:"#",
            }, 
            {
                text:"TV",
                url:"#"
            }, 
            {
                text:"Games",
                url:"#",
            }, 
            {
                text:"Videos",
                url:"#"
            }, 
            {
                text:"News",
                url:"#"
            },
          ],
          /* array 2/4 */
          shop:[
            {
                text:"Shop DC",
                url:"#",
            }, 
            {
                text:"Shop DC Collectibles",
                url:"#"
            },   
          ],
          /* array 3/4 */
          dc:[
            {
                text:"Terms Of Use",
                url:"#",
            }, 
            {
                text:"Privacy policy (New)",
                url:"#"
            },   
            {
                text:"Ad Choices",
                url:"#",
            }, 
            {
                text:"Adcertising",
                url:"#"
            }, 
            {
                text:"Jobs",
                url:"#"
            },
            {
                text:"Subsriptions",
                url:"#",
            }, 
            {
                text:"Talent Worckshops",
                url:"#"
            },   
            {
                text:"CPSC Certificate",
                url:"#",
            }, 
            {
                text:"Rating",
                url:"#"
            }, 
            {
                text:"Shop Help",
                url:"#"
            },  
            {
                text:"Contact Us",
                url:"#"
            }, 
          ],
          /* array 4/4 */
          sites:[
            {
                text:"DC",
                url:"#",
            }, 
            {
                text:"MAD Magazine",
                url:"#"
            },   
            {
                text:"DC Kids",
                url:"#",
            }, 
            {
                text:"DC Universe",
                url:"#"
            }, 
            {
                text:"DC Power Visa",
                url:"#"
            },
          ],
      }
  }
}
</script>
<style scoped lang="scss">
#shop {
    background-color: rgb(0, 200, 255);
    /* debug */
    height: 200px;

    section {
        display: flex;
    }
}
#foot-link {
    background-color: black;
    color: white;
    background-image: url("../assets/img/footer-bg.jpg");
    background-repeat: no-repeat;
    background-size: cover;
    display: flex;
    justify-content: space-between;
    /* debug */
    /* height: 300px; */

    #for-flex {
        display: flex;
        margin: 20px 0;
        width: 45%;
    }
    section {
        display: flex;
        justify-content: space-between;
        width: 70%;
        margin: auto;
    }

    h1 {
        margin: 10px;
    }
    li {
        list-style-type: none;
        margin:  10px;

        a{
            text-decoration: none;
            color: grey;
        }
    }

    figure {
        width: 55%;
        position: relative;
        overflow: hidden;
    }

    figure img {
        width: 500px;
        height: 500px;
        position: absolute;
        top: -50px;
    }
}
#sing-up {
    background-color: rgb(41, 40, 40);
    /* debug */
    /* height: 150px; */

    #bottom-page{
        width: 70%;
        margin: auto;
        display: flex;
        justify-content: space-between;
        align-items: center;
        padding: 20px;

        div h2 {
            color: blue;
        }
        
        button {
            background-color: transparent;
            border: 1px solid blue;
            padding: 15px;
        }

        button h2 {
            color: white;
        }

        div {
            display: flex;
        }

        img {
            margin: 0 15px;
        }
    }
}
</style>
