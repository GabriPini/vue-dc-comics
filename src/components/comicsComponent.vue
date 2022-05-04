<template >
<div class="comic-cover">
  <img :src="comicImage" alt="">
  <p>{{ comicTitle }}</p>
</div>
</template>


<script>
export default {
  props:{
    comicImage: String,
   comicTitle: String
  }

}

</script>

<style lang="scss" scoped>
        .comic-cover{
            flex-basis: calc(100% / 6);
            padding: 10px;
            margin-bottom: 15px;
            img{
                width: 100%;
                height: 150px;
                object-fit: cover;
                object-position: top;
    
            }
    
            p{
                font-size: 0.7rem;
                font-weight: bold;
            }
        }
</style>