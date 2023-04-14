<script>
    import Tilbake from "../tilbake/tilbake.svelte"


</script>

<body>

<h1>Push Day</h1>
	<table>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
			<tr>
				<td>Triceps push-down</td>
				<td>4</td>
				<td>10-15</td>
			</tr>
			<tr>
				<td>Bicep curls</td>
				<td>4</td>
				<td>10-15</td>
			</tr>
			<tr>
				<td>Shoulder press</td>
				<td>3</td>
				<td>8-10</td>
			</tr>
			<tr>
				<td>Hammer curls</td>
				<td>3</td>
				<td>8-12</td>
			</tr>
			<tr>
				<td>Skull crushers</td>
				<td>3</td>
				<td>6-8</td>
			</tr>
            <tr>
                <td>Lateral rasises</td>
                <td>3</td>
                <td></td>
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
