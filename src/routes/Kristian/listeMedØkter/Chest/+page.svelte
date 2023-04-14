<script>
    import Tilbake from "../tilbake/tilbake.svelte"


</script>

<body>

<h1>Chest</h1>
	<table>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
			<tr>
				<td>Bench-press</td>
				<td>4</td>
				<td>5-8</td>
			</tr>
			<tr>
				<td>Incline bench-press</td>
				<td>3</td>
				<td>5-8</td>
			</tr>
			<tr>
				<td>Pec fly</td>
				<td>4</td>
				<td>8-12</td>
			</tr>
			<tr>
				<td>Dips</td>
				<td>4</td>
				<td>8-10</td>
			</tr>
			<tr>
				<td>Push-ups</td>
				<td>3</td>
				<td>MAX</td>
			</tr>
	</table>
</body>

<Tilbake/>

<style>
    table{
        border-collapse: collapse;
    }
    td, th{
       border: 2px solid black; 
    }
    
</style>
