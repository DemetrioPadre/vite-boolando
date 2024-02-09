<script>
export default {
    props: {
        img: String,
        title: String,
    },
};
</script>

<template>
    <div class="card">
        <img :src="img" alt="">
    </div>
</template>

<style lang="scss"></style>