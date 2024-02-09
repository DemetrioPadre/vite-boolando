<script>
export default {
    data() {
        return {

            images: [
                {
                    image: '1.webp',
                    imageHover: '',
                },
                {
                    image: '2.webp',
                    imageHover: ''
                },
                {
                    image: '3.webp',
                    imageHover: ''
                },
                {
                    image: '4.webp',
                    imageHover: ''
                },
                {
                    image: '5.webp',
                    imageHover: ''
                },
                {
                    image: '6.webp',
                    imageHover: ''
                },
            ],
        };
    },
    methods: {
        buildImagePath(imageName) {
            const imageUrl = new URL('../assets/img/' + imageName, import.meta.url).href;
            return imageUrl.href;
        }

    }
};
</script>
<template>
    <div v-for="image in images">
        <img :src="buildImagePath(image)" alt="">
    </div>
</template>
<style lang="scss"></style>