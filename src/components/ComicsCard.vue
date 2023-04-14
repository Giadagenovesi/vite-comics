<script>
export default {
    name: "ComicsCard",
    props: {
        img: String,
        series: String,
    }
}
</script>

<template>
    <div class="card">
        <img :src="img" alt="">
        <h4>{{ series }} </h4>
    </div>
</template>

<style>
    .card {
        width: calc(100% /6 - 20px);
        margin: 10px;
    }
    .card img {
        width: 100%;
        height: 180px;
    }
</style>