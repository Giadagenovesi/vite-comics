<script>
import ComicsCard from "./ComicsCard.vue"

export default {
    components: {
        ComicsCard,

    },
    data () {
    return {
      comics: [
                {
                    thumb: 'https://www.coverbrowser.com/image/action-comics/1-1.jpg',
                    price: '$19.99',
                    series: 'Action Comics',
                    type: 'comic book',
                },
                {
                    thumb: 'https://www.panini.it/media/catalog/product/cache/a5b5dd3adfe0d321084804c738f29601/M/1/M1BLLA015ISBN_0.jpg',
                    price: '$3.99',
                    series: 'American Vampire 1976',
                    type: 'comic book',
                },
                {
                    thumb: 'https://media.wired.com/photos/593384dad80dd005b42b2817/master/w_2560%2Cc_limit/Aquaman-16.jpg',
                    price: '$16.99',
                    series: 'Aquaman',
                    type: 'graphic novel',
                },
                {
                    thumb: 'https://d29xot63vimef3.cloudfront.net/image/batgirl/1-1.jpg',
                    price: '$2.99',
                    series: 'Batgirl',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.posters.cz/image/750/locandine-film-in-plexiglass-batman-prowl-comic-cover-i69653.jpg',
                    price: '$3.99',
                    series: 'Batman',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/5/50/Batman_Beyond_v.1_1.jpg',
                    price: '$2.99',
                    series: 'Batman Beyond',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/0/0d/Batman_Superman_Vol_1_1.jpg',
                    price: '$3.99',
                    series: 'Batman/Superman',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/c/cf/Batman_Superman_Annual_Vol_2_1.jpg',
                    price: '$4.99',
                    series: 'Batman/Superman Annual',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/5/54/Batman_The_Joker_War_Zone_Vol_1_1.jpg',
                    price: '$5.99',
                    series: 'Batman: The Joker War Zone',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/6/64/Batman_Three_Jokers_Collected.jpg',
                    price: '$6.99',
                    series: 'Batman: Three Jokers',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/f/f8/Batman_White_Knight_Presents_Harley_Quinn_Vol_1_1.jpg',
                    price: '$4.99',
                    series: 'Batman: White Knight Presents: Harley Quinn',
                    type: 'comic book',
                },
                {
                    thumb: 'https://static.wikia.nocookie.net/marvel_dc/images/c/c8/Catwoman_Vol_2_1.jpg',
                    price: '$16.99',
                    series: 'Catwoman',
                    type: 'graphic novel',
                },
            ]
    }
  },
    name: "AppMain",
}
</script>

<template>
    <main>
        <section class="jumbotron">
            <div >
                <a class="series-btn" href="">
                    CURRENT SERIES
                </a>
            </div>
        </section>
        <section class="comics">
            <div class="container">
                <div class="row">
                    <ComicsCard v-for="(comic, index) in comics" :key="index" :img="comic.thumb" :series="comic.series" />
                </div>
            </div>
        </section>
    </main>
    
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;

.jumbotron {
    height: 320px;
    background-image: url(../assets/img/jumbotron.jpg);
    background-size: cover;
    position: relative;
    .series-btn {
        background-color: #0282F9;
        color: white;
        display: inline-block;
        text-decoration: none;
        font-weight: bold;
        padding: .8rem 1rem;
        position: absolute;
        bottom: -20px;
        left: 220px;
    }
}
.comics {
    background-color: #1C1C1C;
    color: white;
    padding: 3rem 0;

    .row {
       display: flex;
       flex-wrap: wrap;
    }
}

</style>