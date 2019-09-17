<template>
<div>
    <h3>section two</h3>
    <input type="text" :value="product.price"> <input type="text" :value="product.num">
</div>
</template>

<script>
export default{
    name: 'SectionTwo',
    props: ['product'],

}
</script>