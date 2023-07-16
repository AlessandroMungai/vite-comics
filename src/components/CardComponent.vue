<script>
export default {
    name: 'CardComponent',

    data(){
        return {

        }
    },
    props: {

        cardImg:String,
        cardTitle:String,
        cardSubtitle:String,
        cardPrice:Number

    },
}
</script>

<template>

    <div class="card">

        <img :src="cardImg" :alt="cardTitle">

        <p class="title-series">
            {{cardTitle}}
        </p>
        <p class="type-series">
            {{cardSubtitle}}
        </p>
        <p class="price-series">
            {{cardPrice}}
        </p>

    </div>

</template>

<style scoped lang="scss">

    img {
        width: 180px;
        height: 180px;
        object-fit: cover;
        object-position: top;
        transition: all 0.3s ease-in-out;
    }

    img:hover {
            transform: scale(1.1);
        }
    .card {

        width: calc(100% / 6 - 10px);
        margin: 5px 5px;
        cursor: pointer;

    }
    
    p {
        &.title-series {
            color: white;
            text-transform: uppercase;					
        }
        &.type-series {
            color: #0D7CEC;
            font-style: italic;
            font-size: 0.9rem;
        }
        &.price-series {
            color: #e1ec0d;
            font-size: 0.8rem;
        }
    }

</style>
