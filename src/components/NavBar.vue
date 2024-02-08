<template>
    <header>
        <div class="helper">
        
        </div>

        <div class="meuLogo">
          <h1>Erick Henrique<span>.</span></h1>
          <p class="pipe">|</p>
          <nav>
            <ul>
              <li><a>Home</a></li>
              <li><a>Sobre</a></li>
              <li><a>Projetos</a></li>
              <li><a>Contato</a></li>
            </ul>
          </nav>
        </div>

        <nav>
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
  header {
    display: flex;
    justify-content: space-between;
    align-items: center;
    height: 80px;
    background-image: linear-gradient( to right, #0E041D, #150323);
  }

.meuLogo{
  display: flex;
  align-items: center;
  h1{
    margin: 0;
    font-size: 2rem;
    margin-left: 4rem;
    margin-right: 1rem;
    font-weight: 800;

    span{
      color: red;
    }
  }

  .pipe{
    margin: 0;
    font-size: 2rem;
    font-weight: 100;
  }

  nav ul{
    margin: 0;
    display: flex;
    list-style: none;
  }

  nav ul li a{
    margin: 0 40px;
    cursor: pointer;
    font-size: 1.5rem;
    font-weight: 300;
  }
}

.sideMenu {
  display: none;
}


.helper{
  display: none;
}

header img {
  width: 180px;
}

nav{
  display: flex;
  align-items: center;
  margin-right: 40px;
  }

nav a{
  margin: 0 20px;
  cursor: pointer;
}

nav a img{
  width: 30px;
}

@media (hover: hover) {
  nav ul li a:hover {
    color: #00f;
  }

}

/* media quero smartphone */


@media (max-width: 1024px) {
  nav{
    display: none;
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
  }

  .sideMenu {
    display: flex;
    img {
      width: 3rem;
    }
  }
}

</style>
