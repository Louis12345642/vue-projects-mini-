<template>
<div class="day">
    <div class="day-name-wrapper">
        <h2>{{day.abbvTitle}}</h2>
    </div>
    
    <div class="number-wrapper">
        <p>{{day.id}}</p>
       
    </div>
    <calender-event v-for="event in day.events"  :event="event"/>    
    

</div>
</template>
<script>
import calenderEvent from "./calenderEvent.vue"

export default{
    name:"calenderDay",
  data(){
    return{

    }
    
  },
  components:{
   calenderEvent,
  },
props:['day']
}
</script>
<style>
.day{
    background-color:rgb(70, 68, 68);
    height:700px;
}
.day-name-wrapper{
    background-color: rgb(54, 51, 51);
    color: #fff;
    text-align: center;
    height:40px;
    display:flex;
    align-content:center;
    justify-content: center;
    padding: 6px;
    text-transform:scapitalize;
    font-family: 'Roboto', sans-serif
}
.number-wrapper{
    display: flex;
    height:50px;
    align-content: center;
    padding:20px;
    gap:20px;
    color: #fff;
    font-size: 25px;
}



</style>