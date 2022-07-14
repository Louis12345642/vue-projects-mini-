<template>

<calender-week/>
<calender-entry/>
</template>
<script>
import calenderWeek from "./components/calenderWeek.vue"
import calenderEntry from "./components/calenderEntry.vue"
export default{
  name:"App",
  components:{
    calenderWeek,
    calenderEntry
  }
}
</script>
<style>
*{
  margin:0;
  padding:0;

}
body{
  background-color: rgb(168, 164, 164);
}

</style>