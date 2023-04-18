<script>
  let ikkeInnlogget = true;
  let innlogget = false;
  let innlogget2 = false;
  let ferdig = false;
  let godtaFullført = false;
  let visKlokke = false
  const side0 = () => {
    ikkeInnlogget = true;
    innlogget = false;
    visKlokke = false;
  };

  const side1 = () => {
    innlogget = true;
    innlogget2 = false;
    ikkeInnlogget = false;
    visKlokke = true;
  };
  const side2 = () => {
    innlogget2 = true;
    innlogget = false;
    ikkeInnlogget = false;
    godtaFullført = false;
  };
  const fullførtSjekk = () => {
    innlogget2 = false;
    innlogget = false;
    ikkeInnlogget = false;
    ferdig = false;
    godtaFullført = true;
  };
  const ferdigside = () => {
    innlogget2 = false;
    innlogget = false;
    ikkeInnlogget = false;
    ferdig = true;
    godtaFullført = false;
  };
  import Stopwatch2 from "./Stopwatch/stopwatch2.svelte";
</script>

<div class="container">
    <div class="venstre">
          <div class="litenVenstre">
      {#if ikkeInnlogget}
        <button on:click={side1} id="startKnapp"> Start økt</button>
      {/if}
      {#if innlogget}
        <h1>Øvelse 1</h1>
        <p>Pushups</p>
        <p>Antall repetisjoner: 20</p>
        <div class="knappContainer">
        <button on:click={side0}>Tilbake </button>
        <button on:click={side2}>Neste øvelse </button>
      </div>
      {/if}
      {#if innlogget2}
        <h1>Øvelse 2</h1>
        <p>Situps</p>
        <p>Antall repetisjoner: 15</p>
        <div class="knappContainer">
        <button on:click={side1}>Tilbake </button>
        <button on:click={fullførtSjekk}>Fullfør økt </button>
      </div>
      {/if}
      {#if godtaFullført}
        <h1>Er du helt sikker?</h1>
        <button on:click={side2}>Avbryt </button>
        <div class="knappContainer">
        <button on:click={ferdigside}>Godta </button>
      </div>
      {/if}
      {#if ferdig}
        <h1>Bra jobba! Du er nå ferdig med økten.</h1>
      {/if}
    </div>
</div>
  
{#if visKlokke}
  <div class="hoyre"><Stopwatch2 /></div>
  {/if}
</div>

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
#startKnapp{
      position: absolute;
      right: 50%;
}
  h1 {
    font-size: 24px;
    margin-bottom: 10px;
  }

  p {
    font-size: 18px;
    margin-bottom: 5px;
  }

  body {
    font-family: Arial, sans-serif;
    text-align: center;
    margin: 0;
    padding: 0;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    height: 100vh;
    background-image: url("");
    background-size: cover;
    background-position: center;
    background-repeat: no-repeat;
  }

  button:nth-of-type(1) {
    background-color: white;
    color: #007bff;
    border: 2px solid #007bff;
  }
  .container {
    display: flex;
    flex-direction: row;
    width: 100%;
  }
  .venstre {
    width: 50%;
    display: flex;
    flex-direction: column;
    padding: 30vh;

  }
  .litenVenstre{
        display: flex;
        flex-direction: column;
        align-items: center;
  }
  .knappContainer{
        display: flex;
        flex-direction: row;
  }
  .hoyre {
    width: 50%;
    display: flex;
  }

</style>
