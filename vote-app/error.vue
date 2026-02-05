<script setup lang="ts">
import type { NuxtError } from '#app';

const {error} = defineProps<{error: NuxtError}>();
</script>

<template>
    <div class="error">
        <div class="error-wrapper">
            <h1 class="error-code">{{ error.status }}</h1>
            <div v-if="error.status === 404" class="error-message">Страница не найдена, вернитесь на главную страницу</div>
        </div>
        <MainButton class="error-button">На главную</MainButton>
    </div>
</template>

<style scoped>
    .error {
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        gap: 35px;
        min-height: 100vh;
    }

    .error-wrapper {
        display: flex;
        flex-direction: column;
        align-items: center;
        gap: 30px;
    }

    .error-code {
        margin: 0;
        font-size: 120px;
        font-weight: 500;
    }
    
    .error-message {
        color: var(--color-dark);
        font-weight: 300;
    }
    
    .error-button {
        width: 100%;
        max-width: 301px;
    }
</style>