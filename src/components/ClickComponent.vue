<template>
  <button :href="link">{{ msg }}</button>
</template>

<script>
export default {
    name:'ButtonClick',
    props:{
        msg:String,
        link:String,
        color:String
    }
}
</script>

<style>

</style>