<template>
  <div>

  </div>
</template>

<script>
import emitter from './utils/eventbus';

export default {
    created() {
        emitter.on("chou", (params) => {
            console.log("HomeContent", params)
        })

        // 取消监听时，可以需要先定义函数，不要直接在这里写函数
        emitter.off("off", functionA)
    }
}
</script>

<style scoped>

</style>