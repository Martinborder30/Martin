
<!--Link til font-awesome-->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">


<!-----------------------------------------------------Framside------------------------------------------------>
<div id="framside-main">
    <div id="framside-hoved">
        
        <div id="framsideVenstre"></div>
        <div id="framside_hoyre">
            <!--Navigasjonbar-->
            <div id="omOssContainer">
                <h1 id="omOssTittel">GymHero</h1>
                
                <div id="knapperContainer">
                    <div class="alleKort"><div class="alleKortIndreDiv">Velg program</div></div>>
                    <div class="alleKort"><div class="alleKortIndreDiv">Lag program</div></div>
                </div>
            </div>
        </div>
        <div id="framside_hoyreHoyre"></div>
    </div>
</div>
<!-----------------------------------------------------Footer------------------------------------------------>
<footer id="footer">
    <div id="footerDiv">
        <h1>Support</h1>
        <p>Ved å gi støtte gir det muligheter til å fortsette med å lage nettsider. Det kan man gjøre ved å gi støtte moralsk, ved å følge, eller støtte ved gaver gjennom nummeret under. </p>
        <ul id="sosialeMedier">
            <li><a href="#"><i class="fa fa-facebook"></i></a></li>
            <li><a href="#"><i class="fa fa-google"></i></a></li>
            <li><a href="#"><i class="fa fa-twitter"></i></a></li>
            <li><a href="#"><i class="fa fa-youtube"></i></a></li>
            <li><a href="#"><i class="fa fa-instagram"></i></a></li>
        </ul>
        <p id="vippsNummer">90022635</p>
    </div>
    <div id="under_footer">
        <p>Last updated on 20 Februar 2022 by Martin Ravndal (High School Tryggheim, B.A. in IT/project. In-IT-house writer at TermsFeed)</p>
    </div>
</footer>
<style>
    @import url('https://fonts.googleapis.com/css2?family=Nunito&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Raleway:wght@300&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Montserrat:wght@500&display=swap');
@import url('https://fonts.googleapis.com/css2?family=Shadows+Into+Light&display=swap');
html {
    height: 100%;
}
#bodyId {
    font-family: 'Nunito', sans-serif;
    min-height: 100%;
    margin: 0;
    display: flex;
    flex-direction: column;
}
header h1, h2, h3{

    font-weight: 500;
    font-size: 70px;
    color: #4b4747;
}

/*---------------------------------framside-----------------------------*/
#framside-main{
    display: block;
}

#framside-hoved{
    display: flex;
    flex-direction: row;
    height: 100vh;
    background:url("https://wallpaperaccess.com/full/674849.jpg") center;
    background-size: cover;
    background-attachment: fixed;
}
#framside_hoyreHoyre{
width: 40%;
}
#framsideVenstre{
    width: 40%;
}
#framside_hoyre{
    width: 100%;
    height: 100%;
    background: rgba(0,0,0,0.2);
    display: flex;
    flex-direction: column;
}

#omOssContainer{
    color: #dedcdc;
    width: 100%;
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding-top: 5vh;
    line-height: 3vh;
    font-family: 'Raleway', sans-serif;
    font-size: 2vh;
    
}
#omOssTittel{
    font-family: arial black;
    display: flex;
    justify-content: center;
    font-size: 80px;
    font-weight: bolder;
    color: rgb(194, 71, 62);
    
}
#knapperContainer{
    width: 100%;
    display: flex;
    justify-content: space-around;
    margin-top: 50vh;
}

.alleKort{
        background-color: #2e2e2e;
        margin: 2vh;
        border-radius: 1.5vh;
        padding: 0;
        box-shadow: 20px 20px 20px rgba(240, 240, 240, 0.5);
        transition: 0.2s;
    }
    .alleKort:hover{
        box-shadow: 20px 20px 40px rgba(255, 255, 255, 0.8);
    background: #6d6d6d;
    }
    .alleKortIndreDiv {
        background-color: #d1d1d1;
        padding: 3vh;
        margin: 1vh 3vh;
        border-radius: 1.5vh;
        color: #161616;
        font-family: Tahoma;
        font-size: 2.5vh;
        margin: 10px 0 0 10px;
    }
.homeButtonId{
    padding: 10px 20px;
    background-color: #4b4747;
    color: #f6f2e8;
    border: none;
    border-radius: 50px;
    transition: all 0.3s ease 0s;
    cursor: pointer;
    border: black;
    font-size: 2vh;
    text-decoration: none;
}
.homeButtonId:hover{
    background-color: #b2a25a;
}
/*---------------------------Felles for alle sider------------------------------*/
#footer{
    width: 100%;
    margin-top: auto;
    clear: both;
    color: #f6f2e8;
    background: #262626;
    padding-top: 40px;
    align-items: center;
    justify-content: center;
    text-align: center;
}
#footerDiv{
    display: flex;
    align-items: center;
    justify-content: center;
    text-align: center;
    flex-direction: column;
}
#footerDiv p{
    line-height: 200%;
    max-width: 900px;
    margin: 30px auto;
    font-size: 14px;
}
#footerDiv h1{
    color: #f6f2e8;
    text-transform: capitalize;
}
#sosialeMedier{
    list-style: none;
    display: flex;
    flex-direction: row;
    margin: 30px;
}
#sosialeMedier li{
    margin: 0 10px;
}
#sosialeMedier a i{
    color: #f6f2e8;
    font-size: 30px;
}
#sosialeMedier a:hover i{
    color: #266175;
}
#under_footer{
    font-size: 14px;
    background: black;
}
#under_footer p{
    padding: 20px;
}
</style>