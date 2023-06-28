<script>
export default {
    props:{
        comic: Object
    }
}
</script>

<template>
    <div>
        <div class="card">
            <div class="img">
                <img :src="comic.thumb" :alt="comic.series">
            </div>
            <div class="text">
                {{comic.series}}
            </div>
        </div>
    </div>
</template>

<style lang="scss" scoped>
    .card{
    img{
        width: 100%;
        height: calc((100vw * 70 / 100) / 6 - 15px);
        object-fit: cover;
        object-position: 0 0;
    }
    .text{
        text-transform: uppercase;
        font-size: 10px;
        margin-top: 15px;
    }
  }
</style>