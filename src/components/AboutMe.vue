<template>
    <div class="containerAbout">
        <div class="aboutMe">
          <div class="aboutImage">
              <img src="@/assets/AboutmeImg.svg" alt="Logo" />
          </div>
          <div class="aboutContent">
              <h2>Deixe-me apresentar</h2>
              <p>
                  I am a web developer, I have been working with web development for 2 years, I am passionate about technology and I am always looking for new challenges and learning new technologies.<br>
                  I am a web developer, I have been working with web development for 2 years, 
              </p>
          </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'AboutMe',
    
}
</script>


<style scoped>
  .containerAbout{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 80vh;
  }

  
  .aboutMe {
      display: flex;
      justify-content: center;
      background-color: #1f0b35;
      height: 30rem;
      width: 65rem;
      padding: 20px;
      border-radius: 15px;
  }

  .aboutImage{
      width: 50%;
      display: flex;
      align-items: center;
      justify-content: center;
  }

  .aboutContent {
      width: 50%;
      padding: 1rem;
  }

  .aboutContent h2 {
      font-size: 2rem;
      font-weight: 800;
      line-height: 3rem;
      color: #A110A3;
  }

  .aboutContent p {
      font-size: 1.2rem;
  }


@media (hover: hover) {

}

@media (max-width: 1024px) {
    .aboutMe {
        height: 70vh;
    }
}

@media (max-width: 800px) {
    .aboutMe {
        height: 70vh;
    }
}

/* media query smartphone */

@media (max-width: 600px) {
    .aboutMe {
      text-align: center;
      p {
          font-size: 1.3rem;

      }

      h1 {
          font-size: 2.8rem;
          line-height: 4rem;
          font-weight: 600;
      }
  }
}

</style>
