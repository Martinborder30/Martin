<script>
    import Tilbake from "../tilbake/tilbake.svelte"
</script>

<div>
<h1>Legs</h1>
	<table>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
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
	</table>
</div>

<Tilbake />

<style>
    table{
        border-collapse: collapse;
    }
    td, th{
       border: 2px solid black; 
    }
	div{
		margin: 100px;
	}
    
</style>