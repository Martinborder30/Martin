<script>
	//Importer test filen fra test.svelte
	import Funksjon from "./funksjon.svelte"
//Lager et array og kaller det for personer
//Lager 3 objerkt inni arrayet, og lager ulike verider på de ulike akitviteten
    let personer = [
        {navn: "Første øvelse" ,høydehopp: 2, lengdehopp: 2, hundremeter: 10, totalscore: 10},
       
    ] 
//Lager funksjonen som sorterer arrayet etter totalscoren
//Arrayet får personkopi som nytt navn hver gang det skjer en endring inne i arrayet, endringen blir lagret i en ny"variabel" array med navnetg personkopi.
//Person.slice tar førse objekte i arrayen
//Personkopi.sort samanlikner to verdier/inputs, og sender tilbake den som er størst
$: personerkopi = personer.slice(0);
$: er = personerkopi.sort(function(a,b) {
 return a.hundremeter - b.hundremeter;
 });

</script>
<!-- Each personer as person viser frem en og en verdi fra arrayet
Binner inputfeltene til de ulike objektene-->
<h1>Treningsøkt</h1>
<ul>
  {#each personer as person}
    <li><Funksjon bind:person={person.navn} bind:høydehopp={person.høydehopp} bind:lengdehopp={person.lengdehopp} bind:hundremeter={person.hundremeter} bind:totalscore={person.totalscore}/></li>
  {/each}
  <!-- Kanppen som legger til personer-->
  <button on:click={() => {
    personer=[...personer, {navn: "Ny Øvelse", høydehopp: 0, lengdehopp:0, hundremeter:0,  }]
  }}>
Legg til øvelse
  </button>

</ul>

<div class="tilbake"><a href="/">Tilbake</a></div>






