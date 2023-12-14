<template>
    <section class="pastas">
        <h1>
            --&triangleright; Content goes here &triangleleft;--
        </h1>
        <!-- <article></article> -->
    </section>
</template>

<script>
export default {
    name: 'ListPastas',
    data() {
        return {
            pastaList: []
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;

h1{
    color: $main-content-color;
    text-align: center;
    font-size: 2rem;
}

</style>