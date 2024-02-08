<script setup>
    import { defineProps } from 'vue';
    
    const props = defineProps({
        className: {
            type: String,
            default:'test',
        }
    })
</script>

<template>
    <button :class="className">
        <slot></slot>
    </button>
</template>

<style lang="scss" scoped>
    button {
        padding: 8px 16px;
        border: none;
    }
</style>