<template>
    <header>
        <div class="container">
            <div class="row">

                <div class="col-3 d-flex align-items-center py-3">
                    <img src="@/assets/img/dc-logo.png" alt="">
                </div>

                <div class="col-9 d-flex justify-content-end align-items-center" >
                    <nav class="navbar navbar-light py-0 px-3" v-for="(nome, index) in navElement" :key="index">
                        <a href="#">{{nome.name}}</a>
                    </nav>
                </div>
                
            </div>
        </div>
    </header>
</template>

<script>
export default {
    name: 'HeaderComponent',
    data(){
        return{
            navElement:
            [
        {
            name: 'characters',
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
    header{
        nav{
            a{
                color: #0282F9;
                text-transform: uppercase;
                padding: 51px 0;
                &:hover{
                    border-top: 4px solid white;
                    border-bottom: 4px solid #0282F9;
                }
            }
        }
    }
</style>