<template>
    <section>
        <div class="container py-5">
            <div class="row justify-content-around">
                <div class="col-2">
                    <div class="d-flex justify-content-center align-items-center">
                        <img src="@/assets/img/buy-comics-digital-comics.png" alt="Card image cap">
                        <div class="">
                            <p class="m-0">digital comics</p>
                        </div>
                    </div>
                </div>

                <div class="col-2 d-flex justify-content-center align-items-center">
                    <div class="d-flex justify-content-center align-items-center">
                        <img src="@/assets/img/buy-comics-merchandise.png" alt="Card image cap">
                        <div class="">
                            <p class="m-0">dc merchandise</p>
                        </div>
                    </div>
                </div>

                <div class="col-2 d-flex justify-content-center align-items-center">
                    <div class="d-flex justify-content-center align-items-center">
                        <img src="@/assets/img/buy-comics-subscriptions.png" alt="Card image cap">
                        <div class="">
                            <p class="m-0">subscription</p>
                        </div>
                    </div>
                </div>

                <div class="col-2 d-flex justify-content-center align-items-center">
                    <div class="d-flex justify-content-center align-items-center">
                        <img src="@/assets/img/buy-comics-shop-locator.png" alt="Card image cap">
                        <div class="">
                            <p class="m-0">comic shop locator</p>
                        </div>
                    </div>
                </div>

                <div class="col-2 d-flex justify-content-center align-items-center">
                    <div class="d-flex justify-content-center align-items-center">
                        <img src="@/assets/img/buy-dc-power-visa.svg" alt="Card image cap">
                        <div class="">
                            <p class="m-0">dc power visa</p>
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
            navCardsEelement:
            [
        {
            img: '@/assets/img/buy-comics-digital-comics.png',
            name: 'digital comics',
        },
        {
            name: 'comics',
        },
        {
            name: 'movies',
        },
        {
            name: 'tv',
        },
        {
            name: 'games',
        },
        {
            name: 'collectibles',
        },
        {
            name: 'videos',
        },
        {
            name: 'fans',
        },
        {
            name: 'news',
        },
        {
            name: 'shop',
        },
    ]
        }
    }
}
</script>


<style lang="scss" scoped>
section{
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