@import url("https://fonts.googleapis.com/css2?family=Public+Sans&display=swap");
@import url('https://fonts.googleapis.com/css2?family=Gruppo&family=Quicksand:wght@600&display=swap');

* {
  box-sizing: border-box;
  margin: 0;
  padding: 0;
}

html {
  height: 100%;
}

body {
  font-size: 1.1rem;
  min-height: 10%;
  background-image: url(imagenes/fondo1.png);
  background-size: cover;
}

.grid-container > * {
  padding: 10px;
}

.header {
  grid-area: header;
  background-color: black;
}


.header-logo{
  display: block; 
}


.nav-menu{
  width: 100%;
  height: 30px;
  display: inline-block;
}

li{
  list-style: none;
  display: inline-block;
  float: right;
  margin-left: 10px;
}

li a{
  list-style: none;
  text-decoration: none;
  color: white;
  font-family: 'Gruppo', cursive;
  font-size: 18px;
}

li a:hover{
    border-top: 2px solid white;
}

a h2{
  color: white;
  font-family: ;
  font-size: 20px;
  margin: 5px;
}

h2{
  font-family: 'Gruppo', cursive;
  display: inline-block;
  margin-top: 2px;
}

h3{
  text-align: center;
  font-family: 'Gruppo', cursive;
  font-size: 15px;
}

.main {
  grid-area: main;
  background-color: black;
  width: 100%;
  justify-content: center;
}

.box-artistas{
  width: 100%;
  height: 100%;
  padding: 20px;
  display: flex;
  justify-content: space-around;
  align-items: center;
}

.card-julieta{
  height: 420px;
  border: 1px solid white;
  width: 252px;
}

.card-julieta:hover{
  border-bottom: 5px solid white;
  opacity: 0.9;
  -webkit-transform:scale(1.3);transform:scale(1.01);
  transition: 0.8s;
}

.card-julieta img:hover{
  filter: blur(0.5px);
  transition: 1.8s;
}

.card-julian{
  height: 420px;
  border: 1px solid white;
  width: 252px;
}
.card-julian:hover{
  border-bottom: 5px solid white;
  opacity: 0.9;
  -webkit-transform:scale(1.3);transform:scale(1.01);
  transition: 0.8s;
}

.card-julian img:hover{
  filter: blur(0.5px);
  transition: 1.8s;
}

.card-kabi{
  height: 420px;
  border: 1px solid white;
  width: 252px;
}

.card-kabi:hover{
  border-bottom: 5px solid white;
  opacity: 0.9;
  -webkit-transform:scale(1.3);transform:scale(1.01);
  transition: 0.8s;
}

.card-kabi img:hover{
  filter: blur(0.5px);
  transition: 1.8s;
}

.card-julianna{
  height: 420px;
  border: 1px solid white;
  width: 252px;
}

.card-julianna:hover{
  border-bottom: 5px solid white;
  opacity: 0.9;
  -webkit-transform:scale(1.3);transform:scale(1.01);
  transition: 0.8s;
}

.card-julianna img:hover{
  filter: blur(0.5px);
  transition: 1.8s;
  background-size: cover;
}


.footer {
  position: absolute;
  bottom: 0;
  width: 100%;
  grid-area: footer;
  background-color: black;
  color: white;
  font-size: 15px;
  text-align: center;
}

.grid-container {
  display: grid;
  gap: 10px;
  grid-template:
    "header"  100px
    "."  0px
    "main"    auto
    "." 0px
    "footer"  100px;
}


/*          CELULARES             */

@media (max-width: 600px){

  a.inicio{
    display: none;
  }

  .nav-menu{
    float: none;
    display: block;
    justify-content: center;
    align-content: center;
    width: 100%;
    height: 150px;
  }

  .bio{
    display: block;
    width: 100%;
    justify-content: center;
  }

  .footer {
    grid-area: footer;
    background-color: black;
    color: white;
    font-size: 15px;
    text-align: center;
  }

  .box-artistas{
    margin-top: 50px;
    display: grid;
    width: 100%;
    justify-content: center;
  } 

  .header-logo{
    position: relative;
    top: 10px;
    left: 0;
    display: flex;
    justify-content: center;
  }


  ul{
    display: grid;
    justify-content: center;
    align-items: center;
    align-content: center;
  }

  ul.menu{
    margin-left: 0px;
    padding: 0;
  }

  li{
    margin-top: 10px;
    position: relative;
    float: none;
    display: inline-grid;
    justify-content: space-around;
    width: 100%;
  }


}

/*
@media (max-width: 320px)(max-width: 430px){
  .nav-menu{
    float: none;
    display: block;
    justify-content: center;
    align-content: center;
    width: 100%;
  }

  ul{
    display: flex;
    justify-content: center;
    align-items: center;
    align-content: center;
  }

  .bio{
    display: block;
    width: 100%;
    justify-content: center;
  }

  .footer {
    grid-area: footer;
    background-color: black;
    color: white;
    font-size: 15px;
    text-align: center;
  }

  .box-artistas{
    display: grid;
    width: 100%;
    justify-content: center;
  } 

}


/*          TABLETS            */


@media (max-width: 1047px){
  .grid-container {
    grid-template:
      ".  ." 
      "navbar  navbar" 70px
      "main main"   auto
      "  "  /
      200px    auto;
}
  .nav-menu{
    display: block;
    justify-content: space-between;
    align-content: center;
    width: 100%;
  }

  .header{
    margin-left: 0;
    height: 150px;
    opacity: 0.95;
  }

  .footer{
    position: relative;
  }

  .box-artistas{
      display: grid;
      width: 100%;
      justify-content: center;
      margin-bottom: 40px;
  }
  ul{
    text-align: center;
    justify-content: center;
  }

  li{
    float: none;
    align-items: center;
  }

}


/*          ESCRITORIOS            */

@media (min-width: 1100px) {
    .grid-container {
    grid-template:
      "header  header header"  85px
      ".        main       ."  auto
      "footer  footer footer"  40px /
      0px    auto   0px;
  }

article.main{
    margin-top: 20px;
}

  .footer{
    position: relative;
    flex-wrap: nowrap;
  }

}
