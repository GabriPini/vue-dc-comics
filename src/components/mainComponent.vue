<template>
    <main>
        <section id="jumbotron">
            <h3> -- Content goes here -- </h3>
        </section>       
    </main>
</template>

<script>


export default {
    name: 'SiteMain',
   
}
</script>

<style lang="scss" scoped>
@import '@/style/general.scss';


#jumbotron{
   background-color: $contentBgColor;
    height: 100px;

    h3{
        color: $whiteMainColor;
        padding: 2.5rem 13rem;
    }
}

</style>