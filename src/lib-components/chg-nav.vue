<template>
  <div class="chd-nav">
    <span>{{ title }}</span>
    <a :href="url" v-if="url">{{linkText}}&gt;&gt;</a>
  </div>
</template>

<script>
export default {
    props: {
        title: {
            type: String,
            default: '标题'
        },
        linkText: {
            type: String,
            default: '详情'
        },
        url: {
            type: String,
            default: null
        }
    },
    data: {},
};
</script>

<style scoped>
.chd-nav {
    border-bottom: #999 1px solid;
    width: 100%;
    box-sizing: border-box;
    display: flex;
    align-items: center;
    padding: 20px 30px;
    font-size: 30px;
}
.chd-nav span {
    flex: 1;
}
.chd-nav a {
    font-size: 16px;
}
</style>
