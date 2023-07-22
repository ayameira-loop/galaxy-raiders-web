<template>
  <div id="canvas">
    <div id="deep-space">
    <div id="leaderboard">
      <div class="frame1"> 
        <img src="https://www.logolynx.com/images/logolynx/7f/7fe85fb6677eaf8d18c3511c3fcaad79.png">
      </div> 
        <div class="container">
          <h1>Leaderboard</h1>
        </div>

        <table>
        <tr id="table-header">
            <th><h2>Entry</h2></th>
            <th><h2>Score</h2></th>
            <th><h2><small>#</small>Asteroids</h2></th>
        </tr>
        <tr v-for="score in scores">
            <td>{{ score.startGame }}</td>
            <td>{{ score.score }}</td>
            <td>{{ score.asteroidsDestroyed }}</td>
        </tr>
        </table>

    </div>
    </div>
  </div>
</template>
  
<script>
import leaderboard from "../assets/Leaderboard.json"
export default {
  data: () => ({
    scores: leaderboard
  })
}
</script>

<style>
/* Styles for the leaderboard table */
img {
    height: 200px;
    width: 700px;
    text-align: center;
    margin: auto;
}
.frame1 {
    text-align: center;
    margin: auto;
    z-index: 10;
    margin-top: 35px;
}
.container {
  text-align: center;
}
.leaderboard{
  color:#ddd;
  max-width: 1000px;
  margin-left: auto;
  margin-right: auto;
  padding-left: 10px;
  padding-right: 10px;
}
h2 {
  font-size: 26px;
  margin: 20px 0;
  text-align: center;
  small {
    font-size: 0.5em;
  }
}
li {
    border-radius: 3px;
    padding: 25px 30px;
    display: flex;
    justify-content: space-between;
    margin-bottom: 25px;
}  
table.leaderboard {
  border-collapse: collapse;
  width: 400px;
  margin: 20px auto;
}

/* Styles for table header */
table.leaderboard thead {
  background-color: #f5f5f5;
}

table.leaderboard th {
  padding: 10px;
  font-size: 18px;
  text-align: center;
  border: 1px solid #ddd;
}

/* Styles for table rows */
table.leaderboard tbody tr:nth-child(even) {
  background-color: #f9f9f9;
}

table.leaderboard td {
  padding: 8px;
  font-size: 16px;
  text-align: center;
  border: 1px solid #ddd;
}

/* Style for the first column (Rank) */
table.leaderboard td:first-child {
  font-weight: bold;
  color: #f8fafc; /* Blue color */
} 


</style>