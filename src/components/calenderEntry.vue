<template>
<div class="form-wrapper">
     <form>
        <input type="text" value="" placeholder="New Even">
        <p for="Day">Even day:Monday</p>
        <button>submit</button>
        

     </form>
     
</div>
</template>
<script>
export default{
   name:"calenderEvent"
}

</script>
<style scoped>
.form-wrapper{
   
   display: flex;
   justify-content:center;
   align-content: center;
   margin-top: 100px;
}
form{
  background-color: #fff;
  width:440px;
  height:200px;
  border: 1px solid rgb(100, 224, 255);
  border-radius:10px;
  padding:50px;
  box-shadow: 2px 2px 2px rgba(0, 0n 0, .2);
}
input{
  width:100%;
  border-style:none;
  font-size: 25px;
  border-bottom:3px solid rgb(87, 93, 100);

  font-weight:700;


}
input:focus{
   border-style:none;
    border-bottom:3px solid rgb(87, 93, 100);
}
p{
   padding-top: 40px;
   font-weight: 500;
   font-size:26px;
   font-family: 'Roboto', sans-serif;
   color:rgb(39, 145, 56)
}
button{
   border-style: none;
   margin-top:40px;
    font-weight: 500;
     font-size:20px;
     width:130px;
     height:50px;
     border:1px solid rgb(82, 145, 134);;
   font-family:'Roboto', sans-serif;
   color:rgb(82, 145, 134);
   border-radius:5px;
   
}
</style>