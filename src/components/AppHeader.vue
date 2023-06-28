<script>
export default {
    data(){
        return{
            links: [
                {
                    label: 'CHARACTERS',
                    href: '#',
                    active: false
                },
                {
                    label: 'COMICS',
                    href: '#',
                    active: true
                },
                {
                    label: 'MOVIES',
                    href: '#',
                    active: false
                },
                {
                    label: 'TV',
                    href: '#',
                    active: false
                },
                {
                    label: 'GAMES',
                    href: '#',
                    active: false
                },
                {
                    label: 'COLLECTIBLES',
                    href: '#',
                    active: false
                },
                {
                    label: 'VIDEOS',
                    href: '#',
                    active: false
                },
                {
                    label: 'FANS',
                    href: '#',
                    active: false
                },
                {
                    label: 'NEWS',
                    href: '#',
                    active: false
                },
                {
                    label: 'SHOP',
                    href: '#',
                    active: false
                }
            ]
        }
    }
    
}
</script>

<template>
    <header class="container">
        <div class=" flex justify-between align-center">
            <a href="/">
                <img src="../assets/img/dc-logo.png" alt="">
            </a>
            <ul>
                <li v-for="(link, index) in links" :key="index" :class="link.active ? 'active' : ''">
                    <a :href="link.href">
                        {{ link.label }}
                    </a>
                </li>
            </ul>
        </div>
    </header>
</template>

<style lang="scss" scoped>
    @use '../styles/partials/variables' as *;
    
    .active{
        border-bottom: 5px solid rgb(27,114,232);
    }

    header{

        ul li{
            display: inline-block;
            padding: 30px 20px;
            border-bottom: 5px solid white;

            a{
                font-size: 15px;
                font-weight: 600;
            }

            &:hover{
                border-bottom: $border_bottom_blue;
            }

            &:hover a{
                color: rgb(27,114,232);
            }
        }
    }

    img{
        max-width: 79%;
    }
</style>