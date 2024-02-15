<script setup>
import { useRouter } from 'vue-router';
const props = defineProps(["event"]);
const router = useRouter()
const register = () => {
    // if registration api call is successful
    router.push({
        name: 'EventDetails'
    })
}
</script>

<template>
    <p>Register for the event here</p>
    <button @click="register">Register Me!</button>
</template>
