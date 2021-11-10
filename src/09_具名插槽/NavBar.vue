<template>
  <div class="nav-bar">
      <slot name="default">默认内容</slot>
      <div class="left">
          <slot name="left"></slot>
      </div>
      <div class="middle">
          <slot name="middle"></slot>
      </div>
      <div class="right">
          <slot name="right"></slot>
      </div>
      <div class="additon">
          <!-- v-bind -->
          <slot name="test-dynamic-slotname"></slot>
      </div>
  </div>
</template>

<script>
export default {
    props: {
        name: String
    }
    // data() {
    //     return {
    //         name: "why"
    //     }
    // }
}
</script>

<style scoped>
    .nav-bar {
        display: flex;
    }

    .left,
    .right,
    .additon {
        width: 90px;
        background-color: papayawhip;
    }

    .center {

    }
</style>