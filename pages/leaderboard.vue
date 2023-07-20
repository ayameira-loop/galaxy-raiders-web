<template>
    <div id="leaderboard">

        <div class="container">
          <h1>Leaderboard</h1>
        </div>

        <table class="leaderboard">
        <tr>
            <th>Entry</th>
            <th>Score</th>
            <th># Asteroids</th>
        </tr>
        <tr v-for="score in scores">
            <td>{{ score.startGame }}</td>
            <td>{{ score.score }}</td>
            <td>{{ score.asteroidsDestroyed }}</td>
        </tr>
        </table>


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

.container {
  text-align: center;
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
  color: #007bff; /* Blue color */
}

</style>