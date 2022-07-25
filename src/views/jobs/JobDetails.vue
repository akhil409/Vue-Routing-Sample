<template>
        <div class="jobDetails">
              The path of the Current page is {{id}}
        </div>
</template>

<script>
export default {
    name:'JobDetails',
    props:['id'],
    // data(){
    //     return{
    //         id:this.$forceUpdate.params.id
    //     }
    // }

}
</script>

<style>

</style>