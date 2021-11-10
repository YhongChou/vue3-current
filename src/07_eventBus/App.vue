<template>
  <div>
      <home />
      <about />
      <button @click="addName">+name</button>
  </div>
</template>

<script>
import Home from './Home.vue';
import About from './About.vue';
// import {computed} from 'vue';

export default {
    components: {
        Home,
        About
    },
    provide() {
        return {
            name: "chou",
            age: 3
        }
    }
}
</script>

<style lang="scss" scoped>

</style>>
