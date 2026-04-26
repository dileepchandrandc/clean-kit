<script setup lang="ts">
import type { CleanButtonProps } from '../props';
const prop = withDefaults(defineProps<CleanButtonProps>(), {
    padding: '10px',
    borderRadius: '5px',
    borderSize: '1px'
})
</script>
<template>
    <button class="clean-button">{{ prop.text }}</button>
</template>
<style scoped>
.clean-button {
    padding: v-bind(padding);
    border-radius: v-bind(borderRadius);
    border-width: v-bind(borderSize);
}
</style>