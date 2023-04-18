<script>
    import Tilbake from "../tilbake/tilbake.svelte"


</script>

<div>

<h1>Plyometrics</h1>
	<table>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
			<tr>
				<td>Hope tau</td>
				<td>2</td>
				<td>1 min</td>
			</tr>
			<tr>
				<td>Depth jumps</td>
				<td>4</td>
				<td>10-15</td>
			</tr>
			<tr>
				<td>Box jumps</td>
				<td>4</td>
				<td>10-15</td>
			</tr>
			<tr>
				<td>Lateral hops</td>
				<td>3</td>
				<td>15-20</td>
			</tr>
	</table>
</div>

<Tilbake/>

<style>
    table{
        border-collapse: collapse;
    }
    td, th{
       border: 2px solid black; 
    }
    
</style>
