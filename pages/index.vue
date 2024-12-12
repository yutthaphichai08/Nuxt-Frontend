<template>
    <div class="container">
        <h1>Welcome to the homepage</h1>
        <img src="/public/image/shopping.svg" alt="">
    </div>
</template>

<script setup>
useHead({
  title:"หน้าแรก",
  meta:[
    {name:"description", content:"ร้านค้า,อุปกรณ์คอมพิวเตอร์"}
  ]
})

</script>

<style scoped>
.container {
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
}

img {
    width: 500px;
    height: 500px;
}
</style>