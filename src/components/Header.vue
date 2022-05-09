<template>
<div id="home" class="Navigation">
    <nav class="navbar">
     <div>
       <img src="https://encrypted-tbn0.gstatic.com/images?q=tbn:ANd9GcS5yP0WWKBKr8erTXdidvl32cJwu11JxWyzlg&usqp=CAU"  style="width:20px height:10px"/>
     </div>
     <ul class="nav-links">
       <div class="menu">
         <li><a href="#home">Home</a></li>
         <li><a href="#standingTable">Standings</a></li>
         <li><a href="#info">Info</a></li>
         <li><a href="#contact">Contact</a></li>
       </div>
     </ul>
   </nav>
</div>
</template>

<script>

export default{
    name:'MyHeader',
    props:{ title:{type: String, default: "My app title"},
            author:{type: String, default: "Author Name"}

    },
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
 padding: 20px;
 background-color: teal;
 color: #fff;
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
</style>
