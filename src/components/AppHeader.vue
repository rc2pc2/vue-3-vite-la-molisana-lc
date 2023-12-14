<template lang="">
    <header>
        <h1>
            Header
        </h1>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',

}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


header{
    @include flex(row, center, center);
}
</style>