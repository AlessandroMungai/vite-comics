<script>
import footDcIcon from "../assets/img/dc-logo-bg.png"
export default {
  name: 'FooterNav',
  
  data(){
    return {
        footDcIcon,
        dcComics: [
            {
                name: 'Characters'
            },
            {
                name: 'Comics'
            },
            {
                name: 'Movies'
            },
            {
                name: 'Tv'
            },
            {
                name: 'Games'
            },
            {
                name: 'Videos'
            },
            {
                name: 'News'
            },
        ],

        shops: [
            {
                name: 'Shop DC'
            },
            {
                name: 'Shop DC Collectibles'
            },
        ],

        dc: [
            {
                name: 'Term Of Use'
            },
            {
                name: 'Privacy Police (New)'
            },
            {
                name: 'Ad Choices'
            },
            {
                name: 'Advertising'
            },
            {
                name: 'Jobs'
            },
            {
                name: 'Subscription'
            },
            {
                name: 'CPSC Certificates'
            },
            {
                name: 'Ratings'
            },
            {
                name: 'Shop Help'
            },
            {
                name: 'Contact Us'
            },
        ],

        sites: [
            {
                name: 'DC'
            },
            {
                name: 'Mad Magazine'
            },
            {
                name: 'DC Kids'
            },
            {
                name: 'DC Universe'
            },
            {
                name: 'DC Power Visa'
            },
        ],
    }
  },
  methods: {

  }
}
</script>

<template>

    <footer>
        
        <div class="container">

            <div class="foot-contain">

                <div class="ft-shops">

                    <h4>
                        DC COMICS
                    </h4>

                    <ul>
                        <li v-for="typology in dcComics" :key="typology.name">
                            <a href="#">
                                {{ typology.name  }}
                            </a>
                        </li>
                    </ul>

                    <h4>
                        SHOPS
                    </h4>

                    <ul>
                        <li v-for="typology in shops" :key="typology.name">
                            <a href="#">
                                {{ typology.name  }}
                            </a>
                        </li>
                    </ul>

                </div>


                <div class="ft-info">

                    <h4>
                        DC
                    </h4>

                    <ul>
                        <li v-for="typology in dc" :key="typology.name">
                            <a href="#">
                                {{ typology.name  }}
                            </a>
                        </li>
                    </ul>

                </div>

                <div class="ft-sites-info">

                    <h4>
                        SITES
                    </h4>

                    <ul>
                        <li v-for="typology in sites" :key="typology.name">
                            <a href="#">
                                {{ typology.name  }}
                            </a>
                        </li>
                    </ul>

                    <div class="big-icon-dc">

                        <img :src="footDcIcon" alt="">

                    </div>

                </div>

            </div>

        </div>

    </footer>

</template>

<style scoped lang="scss">

    .big-icon-dc img {
        position: absolute;
        right: 200px;
        top: -26px;
        bottom: 50px;
        width: 450px;
    }

    footer {
        padding: 40px 0;
        background-image: url('../assets/img/footer-bg.jpg');
        background-size: cover;
        overflow: hidden;
        position: relative;
    }

    h4 {
        color: white;
        margin-top: 10px;
    }
    .ft-shops {
        margin-right: 50px;
    }
    .ft-sites-info {
        margin-left: 50px;
    }
    .foot-contain {
        display: flex;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0;
    }

    ul {
        list-style-type: none;
        padding-left: 0;

        li{
            text-align: left;
        }
        
        a {
            color: rgb(208, 208, 208);
            text-decoration: none;
            font-size: 0.7rem;
            font-weight: 200;
        }
    }

</style>