<template>
    <table>
        <tr-component v-for="(rowData, index) in tableData" :key="index" :row-index="index" :row-data="rowData"></tr-component>    
    </table>    
</template>

<script>
import TrComponent from './TrComponent';
export default {
    props: {
        tableData: Array,
    },
    components: {
        TrComponent,
    },
};
</script>

<style>

</style>