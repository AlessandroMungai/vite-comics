<script>
import imgLogo from "../assets/img/dc-logo.png";

export default {
  name: 'HeaderNav',
  components: {

  },
  data(){
    return {
        imgLogo,
        name: "logo-dc",
        navItems: [
            {
                name:'CHARACTERS'
            },
            {
                name:'COMICS'
            },
            {
                name:'MOVIES'
            },
            {
                name:'TV'
            },
            {
                name:'VIDEOS'
            },
            {
                name:'FANS'
            },
            {
                name:'NEWS'
            },
            {
                name:'SHOP'
            },
    ]
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
                            
                            <li v-for="item in navItems">
                                <a href="#">
                                    {{item.name}}
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
        .header-contain {
            display: flex;
            justify-content: space-between;        
            align-items: center;

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

                    &:hover {
                        color: #0C7CEC;
                    }
                }
            }
        }
    }
    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0;
    }

</style>