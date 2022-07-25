<template>
        <div class="jobs">
              <div v-for="job in jobs" :key="job.id">
                <router-link :to="{ name: 'JobDetails', params: {id: job.id} }">
                    <h1>My name is {{job.name}} and my Current Designation is {{job.designation}}</h1>
                </router-link>
                
              </div>
        </div>
</template>

<script>
export default {
    name:'Jobs',
    data(){
         return{
             jobs:[
               {id:1,name:'Akhil',designation:'Sofware Engineer'},
               {id:2,name:'Alladi',designation:'QA Engineer'},
               {id:3,name:'Kumar',designation:'DevOps Engineer'}
             ]
         }
    }

}
</script>

<style>

</style>