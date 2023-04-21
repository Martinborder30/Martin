<script>
    import Tilbake from "../tilbake/tilbake.svelte"


</script>

<body>

<h1>Pull Day</h1>
	<div>
		<table>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
			<tr>
				<td>Pull-ups</td>
				<td>3</td>
				<td>5-10</td>
			</tr>
			<tr>
				<td>Rows</td>
				<td>3</td>
				<td>12-15</td>
			</tr>
			<tr>
				<td>Deadlift</td>
				<td>4</td>
				<td>3-5</td>
			</tr>
			<tr>
				<td>Bicep curls</td>
				<td>4</td>
				<td>10-12</td>
			</tr>
            <tr>
                <td>Lat pull-down</td>
                <td>3</td>
                <td>5-10</td>
            </tr>
	</table>
</div>

<Tilbake/>
</body>
<style>
    table{
        border-collapse: collapse;
    }
    td, th{
       border: 2px solid black; 
    }
    
</style>
