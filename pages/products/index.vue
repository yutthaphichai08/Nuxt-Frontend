<template>
    <div class="container">
        <div v-for="product in data.products">
            <nuxt-link :to="`/products/${product.id}`">
                <h2 class="title">{{ product.title }}</h2>
            </nuxt-link>
            <img :src=product.thumbnail>
        </div>
    </div>
</template>

<script setup>
useHead({
    title: "Demo-Shop | สินค้าทั้งหมด",
    meta: [
        { name: "description", content: "ร้านค้า,อุปกรณ์คอมพิวเตอร์" }
    ]
})

const { data: data } = await useFetch('https://dummyjson.com/products?limit=12')
// console.log(data)

</script>

<style scoped>
.container{
    display: flex;
    flex-wrap: wrap;
    justify-content: center;
}
.container div{
    width: 300px;
    height: 300px;
    margin: 30px 15px;
    background: #333
}
.title{
    color: white;
    text-align: center;
    font-size: 1.2em;
}
.container div:hover{
    background: orange;
}
img{
    width: 300px;
    height: 300px;
}
a{
    text-decoration: none;
}
</style>
