<template>
    <div class="container">
        <h1>About</h1>
        <img src="/public/image/about.svg" alt="">
    </div>
</template>

<script setup>
useHead({
  title:"Demo-Shop | เกี่ยวกับเรา",
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