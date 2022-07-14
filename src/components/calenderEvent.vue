<template>
 
  <section >
    <div :style="getEventBackgroundColor" class="event">
<p>{{event.details}}</p>
<div>
    <div class="icons">
    <i style="color:black" class="fa fa-trash"> </i>
         <i style="color:black" class="fa fa-edit"></i>
    </div>
</div>
    </div>
  </section>
    


</template>
<script>
export default{
    name:"calenderEvent",
    props:[
        "event"
    ],
    computed: {
         getEventBackgroundColor() { 
            const colors = ['#FF9999', '#85D6FF', '#99FF99']; 
            let randomColor = colors[Math.floor(Math.random() * colors.length)];
             return `background-color: ${randomColor}`;
              } 
             }
}

</script>
<style scoped>

.event-wrapper{
 position: relative;      
}
.event{
    background-color: rgb(18, 88, 18);
     width:200px ;
    height:100px;
    font-size: 18px;
    font-weight: 400;
    padding-top: 20px;
    margin-top:30px;
    font-family:'Roboto', sans-serif;
}
.icons{
    display: flex;
    gap: 16px;
    cursor: pointer;
    align-content: center;
    padding-top: 10px;
    justify-content: center;
    font-size: 24px;
}
p{
    text-align: center;
    font-size: 24px;
    font-family: 'Roboto', sans-serif
}
section{
margin-left:94px;
margin-top: 2px;
}

</style>