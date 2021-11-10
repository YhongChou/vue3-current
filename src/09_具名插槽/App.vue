<template>
    <nav-bar :name="name">
        <!-- <button>左边</button>
        <h2>中间</h2>
        <i>右边</i> -->
        <template v-slot:left>
            <button>左边的按钮</button>
        </template>
        <template v-slot:middle>
            <button>中间的按钮</button>
        </template>
        <!-- <template v-slot:right>
            <button>右边的按钮</button>
        </template> -->
        <!-- v-slot: 简写 #-->
        <template #right>
            <button>右边的按钮</button>
        </template>
        <!-- 动态插槽 -->
        <!-- 取的是data里面的name的值 -->
        <!-- <template v-slot:[name]>
            <div>addition 2</div>
        </template> -->
        <!-- 简写 -->
        <template #[name]>
            <div>addition 2</div>
        </template>
    </nav-bar>
</template>

<script>
import NavBar from './NavBar.vue';

export default {
    components: {
        NavBar
    },
    data() {
        return {
            name: "test-dynamic-slotname"
        }
    }
}
</script>

<style>

</style>