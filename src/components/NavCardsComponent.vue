<template>
    <section>
        <div class="container py-5">
            
            <div class="row justify-content-around" >
                <div class="col-2 d-flex" v-for="({img, text},index) in navCardsElements" :key="index">
                    <div class="d-flex justify-content-center align-items-center" >
                        <img :src="require(`@/assets${img}`)" :alt="text">
                        <div class="">
                            <p class="m-0">{{text}}</p>
                        </div>
                    </div>
                </div>
                
            </div>
        </div>
    </section>
</template>

<script>
export default {
    name: 'NavCardsComponent',
    data(){
        return{
            navCardsElements:
            [
        {
            img: '/img/buy-comics-digital-comics.png',
            text: 'digital comics',
        },
        {
            img: '/img/buy-comics-merchandise.png',
            text: 'dc merchandise',
        },
        {
            img: '/img/buy-comics-subscriptions.png',
            text: 'subscription',
        },
        {
            img: '/img/buy-comics-shop-locator.png',
            text: 'comic shop locator',
        },
        {
            img: '/img/buy-dc-power-visa.svg',
            text: 'dc power visa',
        },
    ]
    }
    }
}
</script>


<style lang="scss" scoped>
section{
    position: relative;
    z-index: 1;
    background-color: #0282F9;
    
    img{width: 40px;}
    p{
        text-transform: uppercase; 
        font-size: 12px;
        color: white;
        padding-left: 7px;
        }

}
</style>