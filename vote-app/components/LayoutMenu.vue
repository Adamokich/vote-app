<script setup lang="ts">
import IconExit from './icons/IconExit.vue';
import IconHome from './icons/IconHome.vue';

</script>

<template>
    <div class="menu">
        <div class="menu-wrapper">
            <NuxtLink to="/">
                <IconHome/>
            </NuxtLink>
            <NuxtLink to="/4343">
                <IconExit/>
            </NuxtLink>
        </div>
        <div class="menu-hr"></div>
    </div>
</template>

<style scoped>
.menu {
    display: flex;
}
.menu-wrapper {
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    padding: 48px 28px;
    min-height: 100vh;
}

.menu-hr {
    background-color: var(--color-gray-hr);
    width: 1px;
    min-height: 100vh;
}
</style>