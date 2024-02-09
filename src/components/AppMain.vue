<script>
export default {
    data() {
        return {

            images: [
                {
                    image: '',
                    imageHover: '',
                },
                {
                    image: '',
                    imageHover: ''
                },
                {
                    image: '',
                    imageHover: ''
                },
                {
                    image: '',
                    imageHover: ''
                },
                {
                    image: '',
                    imageHover: ''
                },
                {
                    image: '',
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
    <div>
        <img :src="buildImagePath(img)" alt="">
    </div>
</template>
<style lang="scss"></style>