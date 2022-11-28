<template>
<td>{{Whiskey.Distillery}}</td>
<td>{{Whiskey.Winey}}</td>
<td>{{Whiskey.Sweetness}}</td>
<td>{{Whiskey.Smoky}}</td>
<td>{{Whiskey.Medicinal}}</td>
<td>{{Whiskey.Tobacco}}</td>
<td>{{Whiskey.Honey}}</td>
<td>{{Whiskey.Spicy}}</td>
</template>

<script>

export default{
    name: 'SingleWhiskey',
    props:{
        Whiskey: Array
    }
}
</script>

<style scoped>
td{
    padding: 10px;
    border: 1px solid rgb(190, 190, 190);
}
</style>