<template>
  <div id="app">
    <callToAction
      v-bind:message="messageCallToAction"
    ></callToAction>

    <photoGrid 
      v-for="photo in photos" 
      v-bind:photo="photo" 
      v-bind:key="photo.id"
    ></photoGrid>
  </div>
</template>

<script>
import callToAction from './components/callToAction.vue'
import photoGrid from './components/photoGrid.vue'

export default {
  name: 'App',
  components: {
    callToAction,
    photoGrid
  },
  data: () => {
    return {
      photos: [
        {
          id: 0,
          url: "https://alumni.crg.eu/sites/default/files/default_images/default-picture_0_0.png"
        },
        {
          id: 1,
          url: "https://lh3.googleusercontent.com/proxy/f_2l9B-J5Z9pLLKyl_qzuj_LjFsJkCVX-G-GSq_wjlJ-wBaZBlremNaS_UHoHVjABmho0Dh82efQNhc1N1EBvB6X7lQz6ElKL1utFcwp5EY"
        }
      ],
      messageCallToAction: "call to action"
    }
  }
}
</script>

<style scoped>
</style>
