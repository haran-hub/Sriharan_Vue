<template>
<div id="home" class="Navigation">
    <nav class="navbar">
     <div>
         
         
         
     </div>
     <p id = "para">
       *** "The water was not fit to drink. To make it palatable, we had to add whisky. By diligent effort, I learned to like it.”***

        

     </p>     <ul class="nav-links">
       <div class="menu" style="background-color:">
       </div>
     </ul>
   </nav>
</div>
</template>

<script>

export default{
    name:'MyHeader',
    methods:{
        onClick(){
            console.log("We just clicked")
        }
    }
}

</script>
<style scoped>
.Navigation{
    size: 1vmax;
}
li {
 list-style: none;
}
.navbar {
 display: flex;
 align-items: center;
 justify-content: space-between;
 padding: 10px;
 background-color: rgb(0, 0, 0);
 color: #fff;
 margin-left: auto;
 margin-right: auto;
}
.nav-links a {
 color: #fff;
}
.menu {
 display: flex;
 gap: 1em;
 font-size: 18px;
}
.menu li:hover {
 background-color: #4c9e9e;
 border-radius: 5px;
 transition: 0.3s ease;
}
.menu li {
 padding: 5px 14px;
}
.para{
    text-emphasis-color: black;
}
</style>
