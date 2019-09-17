<template>
<div>
    <h3>section one</h3><input type=text :value="product.price"> <input type=text :value="product.num">
</div>
</template>

<script>
export default{
    name: 'SectionOne',
    props: ['product'],
    mounted() {

    }

}
</script>