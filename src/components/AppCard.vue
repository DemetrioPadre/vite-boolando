<script>
export default {
    props: {
        item: Object,
    },
    methods: {
        generateURL(path) {
            return new URL(path, import.meta.url).href;
        }

    },
};
</script>

<template>
    <div class="card">
        <img :src="generateURL('../assets/img/' + item.frontImage)" :alt="title">
        <p class="heart">&hearts;</p>
        <p class="sale">{{ item.badges.value }}</p>
        <p class="sostenibilità">{{ item.badges.value }}</p>
        <p class="brand">{{ item.brand }}</p>
        <p class="model">{{ item.name }}</p>
        <p class="price">{{ item.price }}</p>
    </div>
</template>

<style lang="scss" scoped>
.brand {
    font-weight: bolder;
    font-size: 15px;
}

.model {
    font-weight: bolder;
    font-size: 20px;
}

.price {
    font-size: smaller;
    font-weight: bold;
    color: red;
}
</style>