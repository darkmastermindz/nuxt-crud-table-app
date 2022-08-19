<template>
  <div>
    <Navbar />
    <TableTemplate />
    <ProductTable />
  </div>

</template>

<script lang="ts">
import Vue from 'vue'
import Navbar from '~/components/Navbar.vue';
import ProductTable from '~/components/ProductTable.vue';

export default Vue.extend({
    name: "IndexPage",
    components: { Navbar, ProductTable }
})
</script>
