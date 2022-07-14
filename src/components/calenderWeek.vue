<template>


<section>
    <div class="week-wrapper">
<calender-day v-for="day in days.seedData
" :key="day.id" :day="day"/>

</div>
</section>
<br>




</template>
<script>
import { store } from '../stores/store'
import calenderDay from './calenderDay.vue'

export default{
      name:"calenderWeek",
    components:{
        calenderDay,
        
    },
    data(){
      return{
        days:store.state
      }
    
    }

}

</script>
<style scoped>


.week-wrapper{
    display:grid;
    grid-template-columns:repeat(auto-fit,minmax(200px,1fr));
    grid-gap:5px;
    margin:20px;
    height:700px;
    align-items: center;
}

</style>