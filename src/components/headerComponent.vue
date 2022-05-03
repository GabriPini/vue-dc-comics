<template>
    <header>
        <section>
            <nav id="main-navbar">
                <div class="main-logo">
                    <a href="#">
                        <img src="@/assets/img/dc-logo.png" alt="main-dc-logo">
                    </a>
                </div>

                <ul>

                    <li v-for="(element, index) in navElement " :key="index">
                        <a :class="{ active : element.current }" href="#"> {{ element.name }} </a>
                    </li>
                    
                </ul>


            </nav>
        </section>
    </header>
</template>

<script>
export default {
    name: 'SiteHeader',
    data() {
        return {
            navElement : [
                {
                    name: 'characters',
                    url : '#',
                    current : false
                },
                {
                    name: 'comics',
                    url : '#',
                    current : true
                },
                {
                    name: 'movies',
                    url : '#',
                    current : false
                },
                {
                    name: 'tv',
                    url : '#',
                    current : false
                },
                {
                    name: 'games',
                    url : '#',
                    current : false
                },
                {
                    name: 'collectibles',
                    url : '#',
                    current : false
                },
                {
                    name: 'videos',
                    url : '#',
                    current : false
                },
                {
                    name: 'fans',
                    url : '#',
                    current : false
                },
                {
                    name: 'news',
                    url : '#',
                    current : false
                },
                {
                    name: 'shop',
                    url : '#',
                    current : false
                },
            ]
        }
        
    }
}
</script>

<style lang="scss" scoped>
@import '@/style/variables.scss';
ul{
    list-style: none;
    li>a{
        text-decoration: none;
        color: $linkColor;
    }
}
#main-navbar{
    display: flex;
    justify-content: space-around;
    align-items: center;
    height: 100px;
    .main-logo{
        padding: 7.5px;
        img{
            width: 75px;
        }
        
    }
    ul{
        display: flex;
        justify-content: space-around;
        flex-basis: calc(100% / 2);
        height: 100%;
        a{
            display: inline-block;
            height: 100px;
            line-height: 100px;
            text-transform: uppercase;
            font-size: 0.85rem;
            font-weight: 600;
            color: black;
            line-height: 100px;
        }
        a.active{
            border-bottom: 4px solid $mainBlueColor;
            color: $mainBlueColor;
        }
    }
}
</style>