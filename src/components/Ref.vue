<template>
    <!-- 用于模板 -->
    <p>ref demo {{ ageRef }} {{ state.name }}</p>
</template>

<script>
import { ref, reactive } from 'vue';

export default {
    name: 'Ref',
    setup() {
        const ageRef = ref(20); // 值类型 响应式
        const nameRef = ref('郭浩0');

        const state = reactive({
            name: nameRef, //用于reactive
        });

        setTimeout(() => {
            console.log('ageRef', ageRef.value);

            ageRef.value = 25; // .value 修改值
            nameRef.value = '郭浩1';
        }, 1500);

        return {
            ageRef,
            state,
        };
    },
};
</script>
