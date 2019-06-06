<template>
<div>
    <h1>Trade or view your Portfolio</h1>
    <h6>You may save & Load you data </h6>
    <h6>Click On 'End Day' to begin a New day</h6>
    <hr>
    <p>Your Founds : {{ funds | currency }} </p>
</div>
</template>

<script>
export default {
    computed : {
        funds (){
            return this.$store.getters.funds;
        }
    }
}
</script>

