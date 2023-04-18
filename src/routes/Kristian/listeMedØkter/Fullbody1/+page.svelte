<script>
    import Tilbake from "../tilbake/tilbake.svelte"


</script>

<div>

<h1>Full body workout</h1>
	<table>
			<tr>
				<th>Treningsøvelse</th>
				<th>Antall sett</th>
				<th>Antall repetisjoner</th>
			</tr>
			<tr>
				<td>Push-ups</td>
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
				<td>Sit-ups</td>
				<td>3</td>
				<td>15-20</td>
			</tr>
			<tr>
				<td>Plank</td>
				<td>3</td>
				<td>30-60 sekunder</td>
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
<script>
       
	let ikkeInnlogget = true
	let innlogget = false
	let innlogget2 = false
	let ferdig = false
	let godtaFullført = false
	let innlogget3 = false
	let innlogget4 = false
	let innlogget5 = false
   const side0 =() => {
	  ikkeInnlogget =true
	  innlogget = false
   }   

	const side1 = () => {
	   innlogget = true
	   innlogget2 = false
	   ikkeInnlogget =false
	  innlogget3= false
	   innlogget4 = false
	   innlogget5 = false
	}
	const side2 = () => {
	   innlogget2 = true
	   innlogget = false
	   ikkeInnlogget = false
	   godtaFullført= false
	   innlogget3= false
	   innlogget4 = false
	   innlogget5 = false
	   
	}
	const side3 = () => {
	   innlogget2 = false
	   innlogget = false
	   ikkeInnlogget = false
	   ferdig = false
	   godtaFullført = false
	   innlogget3 = true
	   innlogget4 = false
	   innlogget5 = false
	}
	const side4 = () => {
	   innlogget2 = false
	   innlogget = false
	   ikkeInnlogget = false
	   ferdig = false
	   godtaFullført = false
	   innlogget3 = false
	   innlogget4 = true
	   innlogget5 = false
	}
	const side5 = () => {
	   innlogget2 = false
	   innlogget = false
	   ikkeInnlogget = false
	   ferdig = false
	   godtaFullført = false
	   innlogget3 = false
	   innlogget4=false
	   innlogget5 = true
	}

	const fullførtSjekk = () => {
	   innlogget2 = false
	   innlogget = false
	   ikkeInnlogget = false
	   ferdig = false
	   godtaFullført =true
	   innlogget5 = false          
	}
	const ferdigside = () => {
	   innlogget2 = false
	   innlogget = false
	   ikkeInnlogget = false
	   ferdig = true
	   godtaFullført = false
	   
	}
  
 </script>
 <body>
{#if ikkeInnlogget}

	<button on:click={side1}> Start økt</button>
   
{/if}
 {#if innlogget}
	<h1>Øvelse 1</h1>
	<p>Push-ups</p>
	<p>Antall repetisjoner: 15-20</p>
	<p>Antall set: 3</p>
	<button on:click={side0}>Tilbake </button>
	<button on:click={side2}>Neste øvelse </button>
 {/if}
  {#if innlogget2}
	<h1>Øvelse 2</h1>
	<p>Squats</p>
	<p>Antall repetisjoner: 20</p>
	<p>Antall set: 3</p>
	<button on:click={side1}>Tilbake </button>
   <button on:click={side3}>Neste øvelse </button>
 {/if}
 {#if innlogget3}
	<h1>Øvelse 3</h1>
	<p>Utfall</p>
	<p>Antall repetisjoner: 15(på hver side)</p>
	<p>Antall set: 3</p>
	<button on:click={side2}>Tilbake </button>
   <button on:click={side4}>Neste øvelse </button>
 {/if}
 {#if innlogget4}
	<h1>Øvelse 4</h1>
	<p>Sit-ups</p>
	<p>Antall repetisjoner: 20</p>
	<p>Antall set: 3</p>
	<button on:click={side3}>Tilbake </button>
   <button on:click={side5}>Neste øvelse </button>
 {/if}
 {#if innlogget5}
	<h1>Øvelse 5</h1>
	<p>Planke</p>
	<p>Antall repetisjoner: 60 sek</p>
	<p>Antall set: 3</p>
	<button on:click={side4}>Tilbake </button>
   <button on:click={fullførtSjekk}>Fullfør økt </button>
 {/if}
 {#if godtaFullført}
	<h1>Er du helt sikker?</h1>
	<button on:click={side5}>Avbryt </button>
   <button on:click={ferdigside}>Godta </button>
 {/if}
 {#if ferdig}
 <h1>Bra jobba! Du er nå ferdig med økten.</h1>
{/if}
</body>
<style>
button {
background-color: #007bff;
color: white;
padding: 10px;
border-radius: 5px;
font-size: 16px;
margin: 10px;
border: none;
cursor: pointer;
}

h1 {
font-size: 24px;
margin-bottom: 10px;
}

p {
font-size: 18px;
margin-bottom: 5px;
}
</style>
