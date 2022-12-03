<script setup>
import { ref } from 'vue'

const inputValue = ref('')
const isDisabled = ref(false)

const toggleDisable = () => {
    isDisabled.value = !isDisabled.value
}
</script>

<template>
<div>
    <input placeholder="Enter text" v-model="inputValue" :disabled="isDisabled"/>

    <div>
        <button @click="toggleDisable">
            Toggle disable
        </button>
    </div>
</div>
</template>

<style scoped>
</style>
