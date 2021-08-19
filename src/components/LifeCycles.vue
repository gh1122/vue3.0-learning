<template>
    <p>生命周期</p>
</template>

<script lang="ts">
import {
    defineComponent,
    onBeforeMount,
    onMounted,
    onBeforeUpdate,
    onUpdated,
    onBeforeUnmount,
    onUnmounted,
} from 'vue';
//defineComponent函数，只是对setup函数进行封装，返回options的对象
export default defineComponent({
    name: 'lifeCycles',
    // 等于 beforeCreate 和 created
    setup() {
        onBeforeMount(() => {
            console.log('onBeforeMount');
        });
        onMounted(() => {
            console.log('onMounted');
        });
        onBeforeUpdate(() => {
            console.log('onBeforeUpdate');
        });
        onUpdated(() => {
            console.log('onUpdated');
        });
        onBeforeUnmount(() => {
            console.log('onBeforeUnmount');
        });
        onUnmounted(() => {
            console.log('onUnmounted');
        });
    },
    //两种周生命周期api不建议共存使用 后续讲解
    // beforeCreate() {
    //     console.log('beforeCreate');
    // },
    // created() {
    //     console.log('created');
    // },
    // beforeMount() {
    //     console.log('beforeMount');
    // },
    // mounted() {
    //     console.log('mounted');
    // },
    // beforeUpdate() {
    //     console.log('beforeUpdate');
    // },
    // updated() {
    //     console.log('updated');
    // },
    // // beforeDestroy 改名
    // beforeUnmount() {
    //     console.log('beforeUnmount');
    // },
    // // destroyed 改名
    // unmounted() {
    //     console.log('unmounted');
    // },
});
</script>
