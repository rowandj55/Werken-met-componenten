<template>
    <br />
    <ChildComponent v-model="sharedMessage" />
    <p>Message from childcomponent: {{ sharedMessage }}</p>
</template>

<script setup>
import {ref} from 'vue';
import ChildComponent from './components/ChildComponent.vue';

const sharedMessage = ref('');
</script>

<!-- <template>
    <br />
    <ChildComponent @updateMessage="handleMessage" />
    <p>Message from childcomponent: {{ message }}</p>
</template>

<script setup>
import {ref} from 'vue';
import ChildComponent from './components/ChildComponent.vue';

const message = ref('');

const handleMessage = newMessage => {
    message.value = newMessage;
};
</script> -->
