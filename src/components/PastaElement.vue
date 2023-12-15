<template>
    <article :data-cooking-time="cookingTime">
        <img :src="imageSrc" alt="">
        <h2>
            {{ title }}
        </h2>
        <p>
            {{ type }}
        </p>
    </article>
</template>

<script>
export default {
    name: 'PastaElement',
    // props: [
    //     'imageSrc',
    //     'title',
    //     'type',
    //     'cookingTime'
    // ]
    props: {
        title : String,
        type : String,
        imageSrc : {
            type: [String, Boolean],
            required: true
        },
        cookingTime : [Number, String],
    }
}
</script>

<style lang="scss">
    article{
        background-color: white;
        width: calc((100% / 4) - .3rem) ;
        margin-right: .15;
        margin-left: .15;
        border: 5px solid magenta;
        text-align: center;


        img{
            width: 100%;
        }
    }
</style>