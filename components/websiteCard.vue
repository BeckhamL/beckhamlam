<template>
  <div>
    <img :src="website.img_url" class="image" />
    <p>{{ website.title }}</p>
  </div>
</template>

<script>
export default {
  props: ["website"]
};
</script>

<style>
.image {
  width: 100%;
}
</style>
