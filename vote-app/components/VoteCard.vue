<script setup lang="ts">
import IconAvatar from './icons/IconAvatar.vue';
import IconDislike from './icons/IconDislike.vue';
import IconLike from './icons/IconLike.vue';
import IconPencil from './icons/IconPencil.vue';
import IconTrash from './icons/IconTrash.vue';

</script>

<template>
    <div class="vote-card">
        <div class="vote-card-header">
            <div class="vote-card-header-name">
                <IconAvatar/>
                <span>PurpleSchool</span>
            </div>
            <div class="vote-card-header-time-info">4 дня назад</div>
        </div>
        <h2 class="vote-card-title">Добавить функцию голосования</h2>
        <p class="vote-card-descr">
            Попробовать добавить в приложение функцию голосования, которая позволит определить, какая фича более полезна, а какая нет. После добавления поста появляется...
        </p>
        <div class="vote-card-actions">
            <div class="vote-card-actions-left">
                <ActionsButton class="vote-card-like">
                    <span>10</span>
                    <IconLike/>
                </ActionsButton>
                <ActionsButton class="vote-card-dislike">
                    <span>3</span>
                    <IconDislike/>
                </ActionsButton>
            </div>
            <div class="vote-card-actions-right">
                <ActionsButton>
                    <IconTrash/>
                </ActionsButton>
                <ActionsButton class="vote-card-change-btn">
                    <IconPencil/>
                    Изменить
                </ActionsButton>
            </div>
        </div>
    </div>
</template>

<style scoped>
.vote-card {
    display: flex;
    flex-direction: column;
    gap: 10px;
}

.vote-card-header {
    display: flex;
    align-items: center;
    gap: 17px;
    font-size: 14px;
    font-weight: 300;
}

.vote-card-header-name {
    display: flex;
    align-items: center;
    color: var(--color-dark);
    gap: 8px;
}

.vote-card-header-time-info {
    color: var(--color-gray-light)
}

.vote-card-title {
    font-size: 22px;
    font-weight: 400;
}

.vote-card-descr {
    width: 100%;
    max-width: 533px;
    font-weight: 300;
    color: var(--color-dark)
}

.vote-card-actions {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.vote-card-actions-left {
    display: flex;
    gap: 15px;
}

.vote-card-actions-right {
    display: flex;
    gap: 20px;
}

.vote-card-like,
.vote-card-dislike {
    display: flex;
    align-items: center;
    gap: 5px;
}

.vote-card-change-btn {
    display: flex;
    align-items: center;
    gap: 6px;
}
</style>