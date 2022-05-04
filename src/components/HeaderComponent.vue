<template>
    <header>
        <div class="container">
            <div class="row">

                <div class="col-3 d-flex align-items-center py-3">
                    <img src="@/assets/img/dc-logo.png" alt="">
                </div>

                <div class="col-9 d-flex justify-content-end align-items-center" >
                    <nav class="navbar navbar-light py-0 px-3" v-for="({text, href}, index) in navElement" :key="index">
                        <a :href="href">{{text}}</a>
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
            text: 'characters',
            href: '#',
        },
        {
            text: 'comics',
            href: '#',
        },
        {
            text: 'movies',
            href: '#',
        },
        {
            text: 'tv',
            href: '#',
        },
        {
            text: 'games',
            href: '#',
        },
        {
            text: 'collectibles',
            href: '#',
        },
        {
            text: 'videos',
            href: '#',
        },
        {
            text: 'fans',
            href: '#',
        },
        {
            text: 'news',
            href: '#',
        },
        {
            text: 'shop',
            href: '#',
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
                color: $primary;
                text-transform: uppercase;
                padding: 51px 0;
                &:hover{
                    border-top: 4px solid $light;
                    border-bottom: 4px solid $primary;
                }
            }
        }
    }
</style>