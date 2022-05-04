<template>
    <section>
        <div class="container py-5">
            
            <div class="row justify-content-around" >
                <div class="col-2 d-flex" v-for="({img, text},index) in navCardsElements" :key="index">
                    <div class="d-flex justify-content-center align-items-center" >
                        <img :src="img" :alt="text">
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
            img: require('@/assets/img/buy-comics-digital-comics.png'),
            text: 'digital comics',
        },
        {
            img: require('@/assets/img/buy-comics-merchandise.png'),
            text: 'dc merchandise',
        },
        {
            img: require('@/assets/img/buy-comics-subscriptions.png'),
            text: 'subscription',
        },
        {
            img: require('@/assets/img/buy-comics-shop-locator.png'),
            text: 'comic shop locator',
        },
        {
            img: require('@/assets/img/buy-dc-power-visa.svg'),
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
    background-color:$primary;
    
    img{width: 40px;}
    p{
        text-transform: uppercase; 
        font-size: 12px;
        color: white;
        padding-left: 7px;
        }

}
</style>