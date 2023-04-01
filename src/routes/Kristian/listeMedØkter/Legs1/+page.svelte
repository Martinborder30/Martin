<script>
    import Tilbake from "../tilbake/tilbake.svelte"
</script>

<body>
<h1>Legs</h1>
	<table>
		<thead>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
		</thead>
		<tbody>
			<tr>
				<td>Calf Raises</td>
				<td>3</td>
				<td>10-15</td>
			</tr>
			<tr>
				<td>Squats</td>
				<td>3</td>
				<td>10-15</td>
			</tr>
			<tr>
				<td>Lunges</td>
				<td>3</td>
				<td>10-15 (på hver side)</td>
			</tr>
			<tr>
				<td>Bulgarian Squats</td>
				<td>3</td>
				<td>30-60 sekunder</td>
			</tr>
		</tbody>
	</table>
</body>

<Tilbake />

<style>
    table{
        border-collapse: collapse;
    }
    td{
       border: 2px solid black; 
    }
    
</style>