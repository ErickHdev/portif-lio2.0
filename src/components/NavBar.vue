<template>
    <header>
        <div class="helper">
        
        </div>

        <div class="meuLogo">
          <h1>Erick Henrique<span>.</span></h1>
          <p class="pipe">|</p>
          <nav class="routes">
            <ul>
              <li><a>Home</a></li>
              <li><a>Sobre</a></li>
              <li><a>Projetos</a></li>
              <li><a>Contato</a></li>
            </ul>
          </nav>
        </div>

        <nav class="socialLinks">
          <div><a> <img alt="Vue logo" src="../assets/LinkedinIcon.png"/>  </a></div>
          <div><a> <img alt="Vue logo" src="../assets/GitHubIcon.png"/>  </a></div>
        </nav>

        <div class="sideMenu">
          <img alt="Vue logo" src="../assets/menuIcon.png"/>
        </div>

    </header>
</template>


<script>
export default {
  
  }
</script>

<style scoped>

  .sideMenu {
    display: none;
  }

  .helper{
    display: none;
  }

  header {
    display: flex;
    position: fixed;
    justify-content: space-between;
    align-items: center;
    width: 100vw;
    height: 80px;
    background-image: linear-gradient( to right, #0E041D, #150323);
    padding-inline: 10%;
    z-index: 1000;
  }

  .meuLogo{
  display: flex;
  align-items: center;
    h1{
      margin: 0;
      font-size: 2rem;
      margin-right: 1rem;
      font-weight: 800;

      span{
        color: red;
      }
    }

  }

  .pipe{
    margin: 0;
    font-size: 2rem;
    font-weight: 100;
  }



  .routes ul{
    margin: 0;
    display: flex;
    list-style: none;
  }

  .routes ul li a{
    margin: 0 2vw;
    cursor: pointer;
    font-size: 1.5rem;
    font-weight: 300;
  }


  .socialLinks {
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 100px;
  }

  .socialLinks a{
    cursor: pointer;
  }

  .socialLinks a img{
    width: 30px;
  }

@media (hover: hover) {
  nav ul li a:hover {
    color: #00f;
  }

}

@media (max-width: 1300px) {
  header{
    padding-inline: 5%;
  }
}

@media (max-width: 1024px) {
  .meuLogo{
    h1{
      font-size: 1.5rem;
      margin-left: 0;
    }
  }

  .routes ul li a{
    margin: 0 2vw;
    cursor: pointer;
    font-size: 1.2rem;
    font-weight: 300;
  }

  .socialLinks a img{
    width: 20px;
  }
}

/* media quero smartphone */


@media (max-width: 800px) {
  .socialLinks{
    display: none;
  }

  .routes{
    display: none;
  }

  .meuLogo{
    h1{
      font-size: 1.5rem;
      margin-left: 0;
    }

    .pipe{
      display: none;
    }
  }

  .helper{
    display: flex;
    width: 40px;
  }

  header{
    display: flex;
    align-items: center;
    justify-content: space-between;
    height: 10vh;
    margin-inline: 0;
    width: 100vw;
  }

  .sideMenu {
    display: flex;
    margin-right: 15px;

    img {
      width: 3rem;
    }
  }
}

</style>
