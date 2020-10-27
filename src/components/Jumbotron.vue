<template>
    <div class="jumbotron">
        <div class="jumbotron-text">
            <img :src="films.roiLion.logo" class="img-fluid d-block" style="max-width: 60%; margin-bottom: 20px;">
            <p class="lead">
                <a class="btn btn-light btn-md" href="#" role="button">Voir<b-icon icon="play-fill"></b-icon></a>
            </p>
        </div>
    </div>
</template>

<script>
export default {
    name: "Carousel",
    props: ['films']
}
</script>

<style>

</style>