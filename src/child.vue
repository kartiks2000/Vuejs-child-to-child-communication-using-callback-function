<template>
  <div>
    <h1>Hello!! I am the first child....</h1>
    <h2>my name is kartik .</h2>
    <h2>i am {{age}} years old .</h2>
    <button @click="changing">change</button>
  </div>
</template>

<script>
export default {
    props:{
        age : Number,
        func : Function,
    },
    methods:{
        changing(){
            this.func();
        }
    }
}
</script>

<style scoped>
    h1{
        color: blue;
    }
    div{
        background-color: burlywood;
        padding: 2rem;
    }
</style>

