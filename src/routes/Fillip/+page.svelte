<p>hei</p>

<script>
 export let person 
 export let høydehopp = 0
 export let lengdehopp = 0
 export let hundremeter = 0
 export let totalscore = høydehopp*5+lengdehopp*5-hundremeter
export let endreNavn = false
export let endringsforslag = ""


//Lager funkjson som rekner ut toltapoeng
// Bruken av Math.abs jør alle negative tal om til positive tal.

const totalpoeng = () => {
        
        høydehopp=Math.abs(høydehopp)
        lengdehopp=Math.abs(lengdehopp)
        hundremeter=Math.abs(hundremeter)
        totalscore = høydehopp*5+lengdehopp*5-hundremeter
    } 
</script>
<!-- Funkjsonen som legger til ny elev
Dette vises når kappen blir trykket på
Når man trykker på lagre, forsvinner input felter, fordi endrenavn=false-->
{#if endreNavn}
<label> Nytt navn: <input type="text" bind:value={endringsforslag}/></label>
<button 
on:click={() =>{
    person = endringsforslag
    endreNavn = false
}}>
lagre
<!-- Npr man trykk på avbryt, forsvinner det også for endrenavn=false-->
</button>
<button on:click={() => (endreNavn = false)}> Avbryt</button>

<!-- Npr endre navn =true kjem input felte opp-->
{:else}
<span>
    <label>{person} <button on:click={() =>{
    endringsforslag=person
    endreNavn=true
}}>
<!-- Lager input feltene-->
Rediger
    </button> meter høydehopp<input type="number" min=0 bind:value={høydehopp} on:change={totalpoeng(høydehopp, lengdehopp, hundremeter)} > </label>
    <label> meter lengdehopp<input type="number" min=0 bind:value={lengdehopp} on:change={totalpoeng(høydehopp, lengdehopp, hundremeter)}></label>
    <label> sekund på  hundremeter<input type="number" min=0 bind:value={hundremeter} on:change={totalpoeng(høydehopp, lengdehopp, hundremeter)} > Du fikk total {totalscore} poeng</label> 

</span>

{/if} 