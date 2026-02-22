<template>
    <button class="button"><slot/></button>
</template>

<style scoped>
.button {
    cursor: pointer;
    color: var(--color-light);
    background-color: var(--color-dark-accent);
    font-weight: 500;
    border: none;
    border-radius: 20px;
    padding: 11px;
    transition: opacity 0.3s;
}

.button:hover {
    opacity: 0.6;
}
</style>