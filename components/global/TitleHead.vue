<template>
  <div class="text-arrival">
    <div class="title-arrival">
      <img class="logo-title" :src="require('../../public/assets/images/' +image1)" width="5%" alt="" />
      <h2>{{title}}</h2>
    </div>
    <img :src="require('../../public/assets/images/icon/' +image2)" alt="" />
  </div>
</template>

<script>
export default {
  name: "Title Head",
  props: ['title','image1','image2'],
};
</script>
