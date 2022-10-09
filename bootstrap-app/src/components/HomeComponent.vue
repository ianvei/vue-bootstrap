<template>
    <b-container>
      <b-row align-v="center" >
        <job-card v-for="job in jobs" :key="job.id" :name="job.name"></job-card>
      </b-row> 
    </b-container>
  </template>
    
<script> 
import JobCardVue from './JobCard.vue'
export default {
  name: 'HomeComponent',
  components: {"job-card": JobCardVue},
  mounted(){
    this.fetchData();

  },
  data(){
    return {
      jobs: []
    }
  },
  methods: {
    async fetchData(){
      const res = await fetch("jobs.json");
      const val = await res.json();
      console.log(val);
      this.jobs = val;
    }
  }
}
</script>

<style>
</style>
    