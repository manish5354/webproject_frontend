<template>
    <div id="standingTable" class="StandingsBox">
        <table>
            <thead>
    <tr>
        <th class="smallTh">
            Position
        </th>
        <th class="LargeTh">
            Team
        </th>
        <th class="smallTh">
            Points
        </th>
        <th class="smallTh">
            Played
        </th>
        <th class="smallTh">
            Won/Lost/Drawn
        </th>
        <th class="smallTh">
            GF/GA
        </th>
        <th class="smallTh">
            Diff
        </th>
    </tr>
</thead >
        <tr v-for="standing in standings" :key="standing.points">
            <SingleTeam :standing="standing"/>          
        </tr>
        </table>
    </div>
    <div class="headerbg" style="text-align: center;">
                STANDING INFO
            </div>
    <div id="info" class="row contact-details">
        <ul>
        <li>Top 4 teams qualify for Champions Leage</li>
        <li>Position 5, 6, 7 qualify for Europa Leage</li>
        <li>Bottom 3 teams are relegated</li>
        </ul>

    </div>
</template>

<script>
import SingleTeam from "./SingleTeam.vue"
export default{
    name:'StandingList',
    components:{
        SingleTeam
    },
    props:{
        standings: Array
    }
}
</script>

<style scoped>
.contact-details {
            background-color: #8FA6CB;
            padding-top: 5px;
            text-align: left;
            padding-left: 20%;
            padding-bottom: 5px;
        }
.headerbg {
            background-color: black;
            padding: 10px;
            color: white;
            font-size: 17px;
            font-weight: 500;
        }
.StandingsBox{
    background-color: aqua;
}
thead{
    background-color: black;
    color: aliceblue;
}
th{
    text-align: center;
    border: 1px solid rgb(190, 190, 190);
}
.smallTh{
    width: 400px;
    height: 60px;
}
.LargeTh{
    width: 800px;
    height: 60px;
}
table{
    border-collapse: collapse;
}
</style>