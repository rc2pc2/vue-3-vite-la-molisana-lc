<template lang="">
    <footer>
        <section class="navigation">
            <div class="logo">
                <img src="../assets/img/la-molisana-logo.png" alt="La Molisana main logo">
            </div>
            <nav id="pastificio">
                <h2>
                    Pastificio
                </h2>
                <ul>
                    <li><a href="#">Il Pastificio</a></li>
                    <li><a href="#">Grano</a></li>
                    <li><a href="#">Filiera</a></li>
                    <li><a href="#">100 anni di pasta</a></li>
                    <li><a href="#">Sartoria della pasta</a></li>
                </ul>
            </nav>
            <nav id="prodotti">
                <h2>
                    Prodotti
                </h2>
                <ul>
                    <li><a href="#">Le classiche</a></li>
                    <li><a href="#">Le Integrali</a></li>
                    <li><a href="#">Le Speciali</a></li>
                    <li><a href="#">Le Biologiche</a></li>
                    <li><a href="#">Le Gluten-free</a></li>
                </ul>
            </nav>
        </section>

        <section class="lower">
            <img src="../assets/img/footer-montagne-bottom.jpg" alt="Sketched mountains image">
        </section>
    </footer>
</template>

<script>
export default {
    name: 'AppFooter'
}
</script>

<style lang="scss" scoped>
@use '../styles/partials/variables' as *;
@use '../styles/partials/mixins' as *;
footer{

    section.navigation{
        width: 45%;
        margin: 0 auto 3rem auto;

        @include flex(row, space-between, center);

        div.logo{
            width: 25%;
        }


        ul{
            list-style-type: none;
            li{
                margin-bottom: .25rem;
            }
        }

        nav h2{
            color: $main-content-color;
            text-transform: uppercase;
            margin-bottom: 1rem;
        }
    }

}
img{
    width: 100%;
}

</style>
