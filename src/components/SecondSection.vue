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

        digitalComics,
        merchandise,
        subscription,
        shopLocator,
        shopVisa,
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

                <a href="#">
                    <img :src="digitalComics" alt="digital comics">
                    <span>DIGITAL COMICS</span>
                </a>
                <a href="#">
                    <img :src="merchandise" alt="merchandise">
                    <span>DC MERCHANDISE</span>
                </a>
                <a href="#">
                    <img :src="subscription" alt="subscription">
                    <span>SUBSCRIPTION</span>
                </a>
                <a href="#">
                    <img :src="shopLocator" alt="shop locator">
                    <span>SHOP LOCATOR</span>
                </a>
                <a href="#">
                    <img :src="shopVisa" alt="shop visa">
                    <span>SHOP VISA</span>
                </a>

            </div>
            
        </div>

    </div>

</template>

<style scoped lang="scss">

    .shops {
        img {
            width: 45px;
            vertical-align: middle;
        }
        span {
            color: white;
            vertical-align: middle;
            padding-left: 5px;
        }
    }

    .second-section {
        background-color: #0282F9;
        padding: 40px 0;
    }

    .shops {
        display: flex;
        justify-content: space-around;
        align-items: center;
    }

    h1 {
        color:white;
        padding: 40px 0;
        font-size: 1.5rem;
    }

    .container {
        max-width: 1100px;
        margin: 0 auto;
        padding: 0;
    }

</style>