<template>
    <!-- <img alt="Vue logo" src="./assets/logo.png" /> -->
    <!-- <HelloWorld msg="Hello Vue 3.0 + Vite" /> -->
    <ToRef />
    <life-cycles />
</template>

<script>
import HelloWorld from './components/HelloWorld.vue';
import LifeCycles from './components/LifeCycles.vue';

import ToRef from './components/ToRef.vue';
export default {
    name: 'App',
    components: {
        HelloWorld,
        LifeCycles,
        ToRef,
    },
};
</script>
