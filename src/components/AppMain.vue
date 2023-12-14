<template lang="">
    <main>
        <ListPastas />
    </main>
</template>

<script>
import ListPastas from './ListPastas.vue';

export default {
    name: 'AppMain',
    components: {
        ListPastas
    }
}
</script>

<style lang="scss" scoped>
    main{
        background-image: url('../assets/img/fondo-pag-speciali.jpg');
        // background-position: center;
        padding: 4rem;
        margin-bottom: 3rem
    }
</style>
