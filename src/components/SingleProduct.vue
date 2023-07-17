<script>
export default {
    data() {
        return {
            active: true
        };
    },
    props: {
        productImage: String,
        productTitle: String
    }
};
</script>

<template>
    <div class="single-product">
        <div :class="{
                'visible-img': active    
            }">
            <img
                :src="productImage"
                :alt="productTitle"
            />
        </div>
        <h2>{{ productTitle }}</h2>
        <button @click="active = !active">
            Mostra/nascondi immagine
        </button>
    </div>
</template>

<style lang="scss" scoped>
img {
    display: none;
}

.visible-img {
    img {
        display: block;
    }
}
</style>
