<script>
import imgLogo from "../assets/img/dc-logo.png";

export default {
  name: 'HeaderNav',
  components: {

  },
  data(){
    return {
        imgLogo,
        name: "logo-dc"
    }
  },
  methods: {

  }
}
</script>

<template>

    <header>

        <div class="container">

            <div class="header-contain">

                <div class="icon-dc-header">
                    <img :src="imgLogo" :alt="name">
                </div>

                <div class="nav-bar">
                    <nav>

                        <ul>
                            
                            <li>
                                <a href="#">
                                    CHARACTERS
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    COMICS
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    MOVIES
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    TV
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    COLLECTIBLES
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    VIDEOS
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    FANS
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    NEWS
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    SHOP
                                </a>
                            </li>

                        </ul>
                    </nav>

                </div>

            </div>

        </div>

    </header>

</template>

<style scoped lang="scss">

    header {
        background-color: white;
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0;
    }

    .header-contain {
        display: flex;
        justify-content: space-between;        
        align-items: center;
    }

    img {
        width: 60px;
        padding: 20px 0;
    }

    ul {
        display: flex;
        list-style-type: none;

        li{
            padding: 0 20px;
    
        }
        
        a {
            color: black;
            text-decoration: none;
            font-size: 0.8rem;
        }
    }

</style>