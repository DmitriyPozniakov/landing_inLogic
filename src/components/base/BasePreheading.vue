<template>
    <div :style="{ background: backgroundColor, color: textColor }"  class="quality">
        {{ text }}
    </div>
</template>

<script>
export default {
    props:{
        text: {
            type: String
        },
        backgroundColor: {
            type: String,
            default: '#1B660D'
        },
        textColor: {
            type: String,
            default: '#fff'
        }
    }
}
</script>

<style scoped>
.quality {
    padding: 8px 16px;
    border-radius: 33px;
    font-family: 'Gilroy-300';
    text-align: center;
    display: inline-block;
    font-size: 2rem;
}
</style>