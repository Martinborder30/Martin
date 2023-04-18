<script>
  let treningsdeler = [
    {
      tittel: "Full body",
      src: "https://www.builtlean.com/wp-content/uploads/2011/09/full-body-workout.jpg",
      link: "/Kristian/listeMedØkter/Fullbody1",
    },
    {
      tittel: "Legs",
      src: "https://legionathletics.com/wp-content/uploads/2019/06/get-bigger-hamstring-muscles.jpg",
      link: "/Kristian/listeMedØkter/Legs1",
    },
    {
      tittel: "Arms",
      src: "data:image/jpeg;base64,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",
      link: "/Kristian/listeMedØkter/Arms",
    },
    {
      tittel: "Chest",
      src: "https://static.wixstatic.com/media/ea496f_52e334c40a99457b895b93060409d0cd~mv2.jpg/v1/fill/w_640,h_392,al_c,q_80,usm_0.66_1.00_0.01,enc_auto/ea496f_52e334c40a99457b895b93060409d0cd~mv2.jpg",
      link: "/Kristian/listeMedØkter/",
    },
    {
      tittel: "Push",
      src: "https://i.pinimg.com/originals/a9/b0/82/a9b0821e3f43b7383ce6d762c5e9711e.jpg",
      link: "/Kristian/listeMedØkter/Push",
    },
    {
      tittel: "Pull",
      src: "https://cdn.shopify.com/s/files/1/1876/4703/articles/shutterstock_658289782_1000x.jpg?v=1627573520",
      link: "/Henrik",
    },
    {
      tittel: "Crossfit",
      src: "https://www.builtlean.com/wp-content/uploads/2011/09/full-body-workout.jpg",
      link: "/Kristian/listeMedØkter/Crossfit",
    },
    {
      tittel: "Plyometric",
      src: "/src/routes/Kristian/listeMedØkter/Bilde/august.png",
      link: "/Kristian/listeMedØkter/Plyometric",
    },
  ];

  let midtpunkt = Math.ceil(treningsdeler.length / 2);
  let oppe = treningsdeler.slice(0, midtpunkt);
  let nede = treningsdeler.slice(midtpunkt, treningsdeler.length);
</script>

<link
  rel="stylesheet"
  href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css"
/>

<body>
  <div id="hvaSkalTrene"><h1>Velg hva du vil trene</h1></div>

  <div id="treningsBokserContainer">
    <div class="bokserHorisontal">
      {#each oppe as del}
        <a href={del.link}
          ><div
            class="treningsBoks"
            style="background: url({del.src}) center;
        background-size: cover;"
          >
            <div class="treningsBoksNavnContainer">
              <p>{del.tittel}</p>
            </div>
          </div>
        </a>
      {/each}
    </div>
    <div class="bokserHorisontal">
      {#each nede as del}
        <a href={del.link}
          ><div
            class="treningsBoks"
            style="background: url({del.src}) center;
        background-size: cover;"
          >
            <div class="treningsBoksNavnContainer">
              <p>{del.tittel}</p>
            </div>
          </div>
        </a>
      {/each}
    </div>
  </div>

  <a href="/"><div class="tilbake"><i class="fa fa-backward" /></div></a>

  <div id="hvorforTrene">
    <h1>Hvorfor trene?</h1>
  </div>
  <div id="hvorforTreneBilde" />
  <div id="hvorforTreneTekst">
    <p>
      Det er flere gode grunner til å trene regelmessig. For det første kan
      trening hjelpe deg med å opprettholde en sunn vekt, styrke muskler og
      bein, og forbedre hjertehelsen. Det kan også øke energinivået ditt,
      forbedre søvnen din og redusere stressnivået. Trening kan også forbedre
      humøret ditt og øke selvtilliten din. Å trene kan også bidra til å
      forebygge en rekke helseproblemer, som diabetes, hjerte- og karsykdommer,
      og kreft. Det er viktig å finne en treningsform som passer deg og
      livsstilen din, slik at du kan opprettholde en jevn treningsrutine og nyte
      alle fordelene som følger med.
    </p>
    <a href="/">Les mer her</a>
  </div>
  <div id="bilde2">

  </div>
</body>

<style>
  html {
    height: 100%;
    margin: 0;
  }
  body {
    display: flex;
    flex-direction: column;
    align-items: center;
    height: 100%;
    background: url("https://d12hfwo7xdmxn8.cloudfront.net/salespages/survey/tinypngopt-img/hero3.jpg")
      center;
    background-size: cover;
    background-attachment: fixed;
    margin: 0;
  }
  #hvaSkalTrene {
    width: 800px;
    background: linear-gradient(to right, white, black);
    border-radius: 10px;
    margin-top: 10vh;
    padding: 20px;
  }
  #treningsBokserContainer {
    display: flex;
    flex-direction: column;
    padding: 50px;
    background-color: rgba(255, 255, 255, 0.5);
    margin: 100px 0;
    border-radius: 10px;
    overflow-x: scroll;
    width: 50%;
    overflow-y: hidden;
  }
  .bokserHorisontal {
    display: flex;
    flex-direction: row;
  }
  .treningsBoks {
    background-color: white;
    margin: 10px;
    width: 35vh;
    height: 35vh;
    border-radius: 2vh;
    border: 3px solid black;
    transition: 0.1s;
  }
  .treningsBoks:hover {
    box-shadow: 2px 2px 4px black;
  }
  .treningsBoksNavnContainer p {
    background-color: rgba(0, 0, 0, 0.8);
    width: 80%;
    border-radius: 0 20px 20px 0;
    padding: 1vh;
    margin-top: 70%;
    color: white;
  }
  .tilbake {
    position: absolute;
    left: 20px;
    top: 20px;
    padding: 10px;
    border-radius: 10px;
    text-decoration: none;
    color: white;
  }
  .tilbake i {
    font-size: 5vh;
    transition: 0.1s;
  }
  .tilbake i:hover {
    font-size: 6vh;
  }
  #hvorforTrene {
    background-color: rgb(255, 255, 255);
    width: 100%;
  }
  #hvorforTrene h1 {
    margin: 80px 100px;
    line-height: 1.5em;
      letter-spacing: 2px;
  }
  #hvorforTreneBilde {
    background: url("https://images.hdqwalls.com/wallpapers/beautiful-morning-in-mountains-4k-pc.jpg")
      center;
    background-size: cover;
    background-attachment: fixed;
    height: 300px;
    width: 100%;
    filter: brightness(0.8);
  }
  #hvorforTreneTekst {
    background-color: rgb(255, 255, 255);
    width: 100%;
    height: 450px;
  }
  #hvorforTreneTekst p{
      margin: 100px 100px 20px 100px;
      font-size: 3vh;
      line-height: 1.5em;
      letter-spacing: 2px;
  }
  #hvorforTreneTekst a{
    font-size: 2vh;
    color: rgb(99, 99, 99);
    margin: 100px;
    transition: 0.1s;
  }
  #hvorforTreneTekst a:hover{
      color: black;
  }

  #bilde2{
    background: url("https://images.hdqwalls.com/wallpapers/winter-snow-trees-mountains-landscape-hdr-4k-aj.jpg")
      center;
    background-size: cover;
    background-attachment: fixed;
    height: 100vh;
    width: 100%;
    filter: brightness(0.8);
  }
</style>
