<script>
	//Importer test filen fra test.svelte
	import Funksjon from "./funksjon.svelte"
//Lager et array og kaller det for personer
//Lager 3 objerkt inni arrayet, og lager ulike verider på de ulike akitviteten
    let personer = [
        {navn: "Første øvelse" ,høydehopp: 2, lengdehopp: 2,},
       
    ] 
//Lager funksjonen som sorterer arrayet etter totalscoren
//Arrayet får personkopi som nytt navn hver gang det skjer en endring inne i arrayet, endringen blir lagret i en ny"variabel" array med navnetg personkopi.
//Person.slice tar førse objekte i arrayen
//Personkopi.sort samanlikner to verdier/inputs, og sender tilbake den som er størst


</script>
<body><!-- Each personer as person viser frem en og en verdi fra arrayet
Binner inputfeltene til de ulike objektene-->
<h1>Lag eget treningsprogram</h1>
<ul>
  {#each personer as person}
    <li><Funksjon bind:person={person.navn} bind:høydehopp={person.høydehopp} bind:lengdehopp={person.lengdehopp} /></li>
  {/each}
  <!-- Kanppen som legger til personer-->
  <button on:click={() => {
    personer=[...personer, {navn: "Ny Øvelse", høydehopp: 0, lengdehopp:0, hundremeter:0,  }]
  }}>
Legg til øvelse
  </button>

</ul>


<table>
  <tr>
      <th>Øvelse</th>
      <th>Antall set</th>
      <th>Antall repitisjoner</th>
    
  </tr> 
  <!-- Lager ny each blokk slik at verdien blir vist en og en-->
   {#each personer as deltaker}
   <tr>
    <td>{deltaker.navn}</td>
    <td>{deltaker.høydehopp}</td>
    <td>{deltaker.lengdehopp}</td>
    
 </tr>

{/each}
</table>
  
</body>

<style>
h1{
  color: white;
}
table {
  color: white;
  border-collapse: collapse;
  width: 100%;
  margin-bottom: 20px;
}

th, td {
  text-align: left;
  padding: 8px;
  border-bottom: 1px solid #ddd;
}

th {
  background-color: #4CAF50;
  color: white;
}

tr:hover {
  background-color: #f5f5f5;
}

button {
  background-color: #4CAF50;
  border: none;
  color: white;
  padding: 10px;
  text-align: center;
  text-decoration: none;
  display: inline-block;
  font-size: 16px;
  margin-bottom: 20px;
  cursor: pointer;
  border-radius: 5px;
}


/* Bakgrunnsstil for hele siden */
body {
  background-image: url("https://img.freepik.com/free-vector/dark-gradient-background-with-copy-space_53876-99548.jpg"); /* Sett inn din egen bildeadresse her */
  background-size: cover;
  background-repeat: no-repeat;
}


</style>






