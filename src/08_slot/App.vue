<template>
  <div>
      <!-- my-slot-cpn就是一个插槽 -->
      <!-- 1 插入html元素 -->
      <my-slot-cpn>
          <button>我是按钮</button>
      </my-slot-cpn>

        <!-- 2 插入文本 -->
      <my-slot-cpn>
          我是文本
      </my-slot-cpn>

      <!-- 3 插入组件 -->
      <my-slot-cpn>
          <my-button></my-button>
      </my-slot-cpn>

    <!-- 4 默认内容,只要有元素就会替换 -->
      <my-slot-cpn>
      </my-slot-cpn>
  </div>
</template>

<script>
import MySlotCpn from './MySlotCpn.vue';
import MyButton from './MyButton.vue';

export default {
    components: {
        MySlotCpn,
        MyButton
    }
}
</script>

<style scoped>

</style>