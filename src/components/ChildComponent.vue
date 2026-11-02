<template>
    <input v-model="message" placeholder="Type something" />
</template>

<script setup>
const message = defineModel();
</script>

<!-- <template>
    <button @click="emitEvent">Send message</button>
</template>

<script setup>
defineProps({
    message: String,
});

const emit = defineEmits(['updateMessage']);
const emitEvent = () => {
    emit('updateMessage', 'New Message from the childcomponent');
};
</script> -->
