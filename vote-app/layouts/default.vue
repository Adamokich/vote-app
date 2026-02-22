<template>
    <div class="layout-content">
        <LayoutMenu/>
        <div class="container">
            <slot/>
        </div>
    </div>
</template>

<style scoped>
.layout-content {
    display: flex;
    align-items: center;
}
</style>