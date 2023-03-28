<script>
    //Importerer css'es frå ein css fil

</script>
<!--Link til font-awesome-->
<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/4.7.0/css/font-awesome.min.css">


<!-----------------------------------------------------Framside------------------------------------------------>
<div id="framside-main">
    <div id="framside-hoved">
        <div id="framside-venstre">
            <img src="https://i.pinimg.com/originals/bd/82/0c/bd820cc1ca5a93760b9780d2910744fd.jpg" alt="logo" id="logoId">
        </div>
        <div id="framside_hoyre">
            <!--Navigasjonbar-->
            <header id="main_navBarId">

                <div id="container_navBarDiv">
                    <div class="child_navBar"><a class="navBarLink1" href="./vurder_tannlege">Vurder Tannlege</a></div>
                    <div class="child_navBar"><a class="navBarLink1" href="./bli_medlem">Bli medlem</a></div>
                    <div class="child_navBar"><a class="navBarLink1" href="./kontakt">Kontakt</a></div>
                    <div class="child_navBar"><a class="navBarLink1" href="./mer_om_oss">Mer om oss</a></div>
                </div>
                <button class="homeButtonId"><a class="navBarLink1" href="./Framside">Home</a></button>
            </header>
            <div id="omOssContainer">
                <h1 id="omOssTittel">Om oss</h1>
                <p>Lorem ipsum dolor sit amet, consectetur adipiscing elit. Integer gravida, urna non gravida convallis, sapien justo ultrices velit, vel dictum lorem ligula sed purus. Morbi pharetra convallis consequat. Nullam accumsan pulvinar lacus, et interdum lectus imperdiet sit amet. Sed sagittis ex a dapibus faucibus. Duis lacinia gravida eros nec commodo. Praesent nec nunc sed ipsum euismod rutrum. Maecenas tincidunt accumsan dolor, et semper turpis facilisis nec. </p>
            </div>
        </div>
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
    background:url("https://www.helsenorge.no/4a1d84/globalassets/bilder/delingsbilder/tannbehandling-fb.png?w=1200&hash=724F121AD3FC3CD123F4A67F8C024A49E9F9168F12DFCC5089C30A4A2CC3A242") center;
    background-size: cover;
    background-attachment: fixed;
}
#framside-venstre{
    width: 50%;
    height: 100%;
    opacity: 0.7;
    background: white;

}
#logoId{
    display: block;
    margin-left: auto;
    margin-right: auto;
    width: 40%;
    padding-top: 150px;

}

#framside_hoyre{
    width: 50%;
    height: 100%;
    background: rgba(0,0,0,0.5);
    display: flex;
    flex-direction: column;
}
#main_navBarId{
    display: flex;
    justify-content: space-between;
    align-items: center;
    padding: 25px 5%;
    font-size: 18px;
    text-decoration: none;
    color: white;
}
.child_navBar{
    display: inline-block;
    padding: 5px 2vh;
    cursor: pointer;
    color: #dedcdc;
    transition: all 0.3s ease 0s;
    position: relative;
    font-size: 2vh;
}
.navBarLink1{
    text-decoration: none;
    color: #dedcdc;
}
.child_navBar::after{
    content: "";
    position: absolute;
    left: 0;
    bottom: 0;
    width: 100%;
    height: 2px;
    background: #b2a25a;

    transform: scaleX(0);
    transform-origin: right;
    transition: transform 250ms ease-in;
}

.child_navBar:hover::after{
    color: #266175;
    font-size: 30px;

    transform: scaleX(1);
    transform-origin: left;
}
#omOssContainer{
    color: #dedcdc;
    width: 60%;
    display: block;
    margin-left: auto;
    margin-right: auto;
    padding-top: 25vh;
    line-height: 3vh;
    font-family: 'Raleway', sans-serif;
    font-size: 2vh;
}
#omOssTittel{
    font-family: 'Raleway', sans-serif;
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