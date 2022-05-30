<template>
  <div class="container">
       <button v-on:click="bilangan++">Button</button>
     <div class="box">
        <h1 v-text="bilangan"> </h1>
        <h4>(Counter angka, tiap button di click 1) </h4>
     </div>
  </div>
</template>
<script>
 export default{
     data(){
         return{
            bilangan:0
         }
     }
       
   }
   </script>
   <style>
  body{
      background-color:#db9b27;
  }
  .container{
       margin:0 auto;
       display:flex;
       justify-content:center;
       align-items:center;
       flex-direction:row;
  }
  button,.box{
    margin-top:150px;
  }
  button{
      margin-right:50px;
      width:150px;
      height:70px;
      background-color:lightskyblue;
      border:1px solid lightskyblue;
      border-radius:10px;
      font-size:16px;
  }
  button:hover{
    border:1px solid black;
  }
  .box{
      background-color:#fff;
      width:380px;
      height:230px;
      border:1px solid black;
  }
  h1,h2{
     color:black;
  }
  .box h1{
      font-size:80px;
  }
   </style>