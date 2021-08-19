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

export default defineComponent({
    name: 'lifeCycles',

    setup() {},

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
