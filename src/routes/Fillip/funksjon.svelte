<script>
    export let person 
    export let høydehopp = 0
    export let lengdehopp = 0
    export let hundremeter = 0
    
   export let endreNavn = false
   export let endringsforslag = ""
   
   
   //Lager funkjson som rekner ut toltapoeng
   // Bruken av Math.abs jør alle negative tal om til positive tal.
   
   const totalpoeng = () => {
           
           høydehopp=Math.abs(høydehopp)
           lengdehopp=Math.abs(lengdehopp)
           hundremeter=Math.abs(hundremeter)
          
       } 
   </script>
   <!-- Funkjsonen som legger til ny elev
   Dette vises når kappen blir trykket på
   Når man trykker på lagre, forsvinner input felter, fordi endrenavn=false-->
   {#if endreNavn}
   <label> Ny øvelse: <input type="text" bind:value={endringsforslag}/></label>
   <button 
   on:click={() =>{
       person = endringsforslag
       endreNavn = false
   }}>
   lagre
   <!-- Npr man trykk på avbryt, forsvinner det også for endrenavn=false-->
   </button>
   <button style="background-color: red;" on:click={() => (endreNavn = false)}> Avbryt</button>
   
   <!-- Npr endre navn =true kjem input felte opp-->
   {:else}
   <span>
       <label>{person} <button on:click={() =>{
       endringsforslag=person
       endreNavn=true
   }}>
   <!-- Lager input feltene-->
   Rediger
       </button> Antall Set<input type="number" min=0 bind:value={høydehopp} on:change={totalpoeng(høydehopp, lengdehopp, hundremeter)} > </label>
       <label> Antall Reptisjoner<input type="number" min=0 bind:value={lengdehopp} on:change={totalpoeng(høydehopp, lengdehopp, hundremeter)}></label>
        
   
   </span>
   
   {/if} 
   
   <style>
       button {
     background-color: #4CAF50;
     color: white;
     font-size: 16px;
     padding: 8px 16px;
     border: none;
     border-radius: 4px;
     cursor: pointer;
   }
   
   
   
   /* Stil for input-feltene */
   input[type="number"] {
     width: 60px;
     font-size: 18px;
     padding: 5px 10px;
     border: 2px solid #ccc;
     border-radius: 5px;
   }
   </style>