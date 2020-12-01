<template>
    <button :class="'chg-btn ' + type ">
        你好,<slot></slot>
    </button>
</template>

<script>
    export default {
        props: {
            type: {
                type: String,
                default: 'default'
            }
        }
    }
</script>

<style scoped>
.chg-btn {
    box-sizing: border-box;
    height: 40px;
    line-height: 40px;
    padding: 0 10px;
    border: #333 1px solid;
    text-align: center;
    background-color: #fff;
    outline: unset;
    font-size: 16px;
}
.primary {
    color: #fff;
    background-color: #0099CC;
    border: unset;
}
</style>