<script>
export default {
    data() {
        return {
            // product: {
            //     src: "https://www.lamolisana.it/wp-content/uploads/2021/06/84-ditale-quadrato.jpg",
            //     titolo: "N.84 Ditale Quadrato",
            //     tipo: "cortissima",
            //     cottura: 12,
            // }
            // productImage: 'https://www.lamolisana.it/wp-content/uploads/2021/06/84-ditale-quadrato.jpg',
            // productTitle: 'Pasta 1',
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
        <div>
            <img
                :src="productImage"
                :alt="productTitle"
            />
        </div>
        <h2>{{ productTitle }}</h2>
    </div>
</template>

<style lang="scss" scoped>
</style>
