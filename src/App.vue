<template>
 <MyHeader title= "Premier League Standings" author="Manish" />
 <StandingList :standings="standings"/>
 <MyFooter/>
 <StandingRules/>
</template>

<script>
import MyHeader from './components/Header.vue'
import StandingList from './components/StandingList.vue'
import MyFooter from './components/Footer.vue'

export default {
  name: 'App',
  components: {
    MyHeader,
    StandingList,
    MyFooter
  },


data(){

  return{
    standings:[]
  }

},


methods:{

  async fetchStandings(){
    const res = await fetch('https://manish-webdb-final.herokuapp.com/api')
    const data = await res.json()
    console.log("Manish")
    console.log(data)
    return data
    }
  },

  async created(){
  this.standings = await this.fetchStandings()
  }
}
</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
body{
  margin: 0px;
  background-color: black;
}
</style>
