<template>
<div class = "alert" v-bind:style ="{'backgroundColor': bgcolor}">
    {{message}}
</div>    
</template>

<script>
export default {
    name: "Alert",
    props:['message','bgcolor']
    
}
</script>

<style scoped>
.alert{
background-color : mistyrose;
}
</style>