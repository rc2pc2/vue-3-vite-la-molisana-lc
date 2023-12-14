<template lang="">
    <header>
        <section class="logo">
            <img src="../assets/img/la-molisana-logo.png" alt="La Molisana main logo">
        </section>
        <nav class="navigation">
            <ul>
                <li v-for="link in navLinks" :class="(link.active) ? 'active' : ''">
                    <a :href="link.url">
                        {{ link.content }}
                    </a>
                </li>
            </ul>
        </nav>
    </header>
</template>

<script>
export default {
    name: 'AppHeader',
    data() {
        return {
            navLinks : [
                {
                    content: 'Home',
                    url: '#',
                    active: false,
                },

                {
                    content: 'Prodotti',
                    url: '#',
                    active: true,
                },

                {
                    content: 'Chi Siamo',
                    url: '#',
                    active: false,
                },

                {
                    content: 'Contatti',
                    url: '#',
                    active: false,
                }
            ],
        }
    },
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;


header{
    @include flex(row, center, center);
    flex-wrap: wrap;
    margin-bottom: 5rem;
    section.logo{
        width: 100%;
        @include flex(row, center, center);
        margin-bottom: 2.5rem;
    }

    nav.navigation > ul{
        @include flex(row, center, center);
        list-style-type: none;

        li{
            margin-right: 1.5rem;
            font-size: 1.1rem;
            padding: .9rem 1.15rem;
            &.active{
                background-color: $header-nav-bg;
            }

            &:hover{
                background-color: $accent-color;
            }
        }
    }
}
</style>