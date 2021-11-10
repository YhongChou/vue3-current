<template>
  <div>
      <!-- <span v-for="item in names" :key="item">
          {{item}}
      </span> -->
      <!-- <template v-for="item in names" :key="item">
          <span>{{item}}</span>
      </template> -->
      <template v-for="(item, index) in names" :key="item">
          <slot :item="item" :index="index"></slot>
      </template>
  </div>
</template>

<script>
export default {
    props: {
        names: {
            type: Array,
            default: () => []
        }
    }
}
</script>

<style>

</style>