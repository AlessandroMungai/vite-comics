<script>
import digitalComics from "../assets/img/buy-comics-digital-comics.png";
import merchandise from "../assets/img/buy-comics-merchandise.png";
import subscription from "../assets/img/buy-comics-subscriptions.png"
import shopLocator from "../assets/img/buy-comics-shop-locator.png"
import shopVisa from "../assets/img/buy-dc-power-visa.svg"

export default {
  name: 'SecondSection',
  components: {

  },
  data(){
    return {
        iconsMain: [
            {
                img: digitalComics,
                name: 'DIGITAL COMICS'
            },
            {
                img: merchandise,
                name: 'DC MERCHANDISE'
            },
            {
                img: subscription,
                name: 'SUBSCRICTION'
            },
            {
                img: shopLocator,
                name: 'COMIC SHOP LOCATOR'
            },
            {
                img: shopVisa,
                name: 'DC POWER VISA'
            },
        ],

    }
  },
  methods: {

  }
}
</script>

<template>

    <div class="second-section">

        <div class="container">

            <div class="shops">

                <a href="#" v-for="(icon, iconIndex) in iconsMain" :key="iconIndex">
                    <img :src="icon.img" alt="digital comics">
                    <span>{{icon.name}}</span>
                </a>

            </div>
            
        </div>

    </div>

</template>

<style scoped lang="scss">
    .second-section {
        background-color: #0282F9;
        padding: 40px 0;
        .shops {
            display: flex;
            justify-content: space-around;
            align-items: center;

            img {
                width: 40px;
                vertical-align: middle;
            }
            span {
                color: white;
                vertical-align: middle;
                padding-left: 5px;
                font-weight:200
            }
        }
    }
    .container {
        max-width: 1100px;
        margin: 0 auto;
        padding: 0;
    }

</style>