<template>
<td style="background-color:#C3E0E5">{{standing.rank}}</td>
<td class="TeamPicText" style="background-color:#DBE8D8"><img class="imageTexPad" v-bind:src= "standing.teamCrest">{{standing.teamName}}</td>
<td style="background-color:#C3E0E5" >{{standing.points}}</td>
<td style="background-color:#d7d9f2">{{standing.matchesPlayed}}</td>
<td style="background-color:#C3E0E5">{{standing.matchesWon_Lost_Dawn}}</td>
<td style="background-color:#d7d9f2">{{standing.goalsFor_Against}}</td>
<td style="background-color:#C3E0E5">{{standing.goalDifference}}</td>
</template>

<script>
export default{
    name:'SingleTeam',
    props:{
        standing: Array
    }
}

</script>

<style scoped>
.TeamPicText{
    text-align: left;
    padding-left: 10px;
}
.imageTexPad{
    padding-right: 20px;
}
td{
    padding: 10px;
    border: 1px solid rgb(190, 190, 190);
}
</style>