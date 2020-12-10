<template>
<div>
    <div>
    <h1>{{header}}</h1>
    </div>
    <button @click="sayhi">Say Hi</button>
    <button @click ="sayGoodBye">Say GoodBye</button>
    <button @click ="sleep">Sleep</button>
</div>
</template>

<script>
export default {
    data : function(){
        return{
            'header' : ''
        }
    },
    methods : {
        sayhi : function(){
            this.header = "Say Hi"
        },
        sayGoodBye : function(){
            this.header = "Say GoodBye"
        },
        sleep : function(){
            this.header = "ZZZzzzz"
        }

    }
    
}
</script>

<style scoped>
h1 {
    font-size : 28px;
    color : cyan;
}
</style>