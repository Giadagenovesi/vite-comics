<script>
export default {
    name: "AppHeader",
    data() {
        return {
            links: [
                {
                    text: "CHARACTERS",
                    current: "false"
                },
                {
                    text: "COMICS",
                    current: "true"
                },
                {
                    text: "MOVIES",
                    current: "false"
                },
                {
                    text: "TV",
                    current: "false"
                },
                {
                    text: "GAMES",
                    current: "false"
                },
                {
                    text: "COLLECTIBLES",
                    current: "false"
                },
                {
                    text: "VIDEOS",
                    current: "false"
                },
                {
                    text: "FANS",
                    current: "false"
                },
                {
                    text: "NEWS",
                    current: "false"
                },
                {
                    text: "SHOP",
                    current: "false"
                },
            ]
        }
    }
}
</script>

<template>
    
        <div class="container">
            <header>
                <div class="logo">
                    <img src="../assets/img/dc-logo.png" alt="dc logo">
                </div>
                <nav>
                    <ul class="header-nav">
                        <li v-for="link in links" > 
                            <a href="">
                                {{ link.text }}
                            </a>
                        </li>
                    </ul>
                </nav>
            </header>
            
        </div>
    
</template>

<style scoped lang="scss">
@use "../style/partials/mixins" as *;
header {
    @include flex (row, space-between, center);
    height: 70px;
    margin: .8rem 0;

    .logo img {
        width: 60px;
    }
    .header-nav {
        list-style: none;
        @include flex (row, space-between, center);

        li {
            margin: 0 .6rem;
            padding: 2.3rem 0;

            a {
                text-decoration: none;
                color: black;
                font-size: .8rem;
            }
            &.active,
            &:hover {
                border-bottom: 4px solid blue;
            }
        }


    }

}
</style>