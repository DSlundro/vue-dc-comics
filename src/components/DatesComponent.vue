<template>

        <div class="col-2 card d-flex flex-wrap">
            <img :src="img" alt="">
            <div class="card-body text-center d-flex flex-column justify-content-between">
                <h5 class="card-title">{{title}}</h5>
                <a href="#" class="btn btn-primary">Buy {{price}}</a>
            </div>
        </div>

</template>



<script>
export default {
    name: 'DatesComponent',
    props:{
        img: String,
        title: String,
        price: String,
    },
}
</script>

<style lang="scss" scoped>
img{
    width: 100%;
    aspect-ratio: 1/1;
}
</style>