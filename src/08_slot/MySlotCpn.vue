<template>
  <div>
      <h2>组件开始</h2>
      <!-- 如果插槽不具名，那么其他地方在使用时，会把内容都插入到插槽中 -->
        <slot>
            <!-- 插槽的默认内容 -->
            插槽1的默认内容
        </slot>

        <slot>
            插槽2的默认内容
        </slot>

        <slot>
            插槽3的默认内容
        </slot>
      <h2>组件结束</h2>
  </div>
</template>

<script>
export default {

}
</script>

<style>

</style>