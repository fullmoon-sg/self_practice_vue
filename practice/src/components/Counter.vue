<template>
<div class="container">
    <div class="counter">
    <div>
        <h1 v-if="counter%2==0" style="color: green;">{{counter}}</h1>
          <h1 v-else style="color: red;">{{counter}}</h1>
    </div>
    <span v-if="counter%2==0" style="color: green margin-left:10px;">Even</span>
    <span v-else style="color: red margin-left:10px;">Odd</span>
    </div>
    <div>
        <button @click="increase" class="btn btn-primary sm3">+</button>
        <button @click="decrease" class="btn btn-primary sm3">-</button>
    </div>
</div>
</template>

<script>
export default {
    data : function() {
        return {
            'counter' : '0', 
        }
    },
    methods : {
        'increase' : function(){
            this.counter++;
        },
        'decrease' : function(){
            this.counter--;
        },
    }
}
</script>

<style scoped>
span{
    font-size : 28px;
}
</style>