<template>
    <div>
        <button @click="btnClick">about按钮点击</button>
    </div>
</template>

<script>
import emitter from './utils/eventbus';

export default {

    methods: {
        btnClick() {
            console.log('about按钮点击');
            emitter.emit("chou", {name: "Lee", age: "5"})
        }
    }
}
</script>

<style scoped>

</style>