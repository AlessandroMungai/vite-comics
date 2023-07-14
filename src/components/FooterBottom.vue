<script>
export default {
  name: 'FooterBottom',
  components: {

  },
  data(){
    return {

    }
  },
  methods: {

  }
}
</script>

<template>

    <div class="footer-bottom">

        <div class="container">

            <div class="ft-bottom-contain">

                <div class="subscrive">

                    <button>

                        SIGN-UP NOW!

                    </button>

                </div>

                <div class="social-icon">

                    <h5>

                        FOLLOW US

                    </h5>

                    <img src="../assets/img/footer-facebook.png" alt="">
                    <img src="../assets/img/footer-twitter.png" alt="">
                    <img src="../assets/img/footer-youtube.png" alt="">
                    <img src="../assets/img/footer-periscope.png" alt="">
                    <img src="../assets/img/footer-pinterest.png" alt="">

                </div>

            </div>

        </div>
        
    </div>

</template>

<style scoped lang="scss">

    .social-icon {
        display: flex;
        align-items: center;

        h5 {
            color: #0282F9;
            font-size: 1rem;
        }

        img {
            width: 25px;
            margin-left: 10px;
        }
    }
    .ft-bottom-contain {
        display: flex;
        justify-content: space-between;
    }

    .footer-bottom {
        background-color: #303030;
        padding: 20px 0;

        button {
            color: white;
            border: 1px solid #0282F9;
            background: none;
            padding: 5px;
            font-size: 0.9rem;
            cursor: pointer;
        }
    }

    .container {
        max-width: 1200px;
        margin: 0 auto;
        padding: 0;
    }

    

</style>