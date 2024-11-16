<template>
    <button class="action-button">
        <slot></slot>
    </button>
</template>

<style scoped>
.action-button {
    border: none;
    border-radius: 28px;
    background: #fff;
    padding: 16px 28px;
    font-family: 'Gilroy-500';
    cursor: pointer;
    display: flex;
    gap: 15px;
    transition: 0.3s ease;
}

.action-button:hover {
    background-color: #cfff65;
}

.action-button:active {
    background-color: #fffefc;
}
</style>