
<script>
export default {
    name : 'ListComponent',
    props:{
        path: String,
        price: String,
        series: String,
        type: String
    }
}
</script>

<template>
        <div class="box">
        <img :src="path" :alt="series">
        <p>{{ series }} </p>
    </div>


</template>


<style lang="scss">
.box {
    width: calc(100% / 6 - 2rem);
    margin: .6rem 1rem;
    p {
        text-align: center;
        text-transform: uppercase;
        color:white;
        font-weight: lighter;
    }
}
</style>