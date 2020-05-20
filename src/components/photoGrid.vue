<template>
  <div class="photoGrid">
    <img :src="photo.url" alt ="" />
  </div>
</template>

<script>
export default {
  name: 'photoGrid',
  props: ['photo']
}
</script>

<style scoped></style>
