<template>
    <div class="containerProjetos">
        <div class="contentProjetos">
            <h1>Projetos</h1>
            <div class="projetos">

                <div class="projeto">
                    <img src="../assets/projetosImgs/Mresgate.png" class="bgProjeto">
                    <div class="Projetoinfo">
                        <h2>Resgate</h2>
                        <div class="techs">
                            <img src="../assets/skillIcons/nextjs.svg" >
                            <img src="../assets/skillIcons/sass.svg" >
                        </div>
                    </div>
                    <div class="ProjetoDesc">
                        <p>Resgate é um projeto que visa ajudar pessoas que estão passando por momentos difíceis, seja por depressão, ansiedade, ou qualquer outro problema psicológico. O projeto foi feito com Next.js e Sass.</p>
                        <button>Visitar</button>
                    </div>
                </div>

                <div class="projeto">
                    <img src="../assets/projetosImgs/Mresgate.png" class="bgProjeto">
                    <div class="Projetoinfo">
                        <h2>Resgate</h2>
                        <div class="techs">
                            <img src="../assets/skillIcons/nextjs.svg" >
                            <img src="../assets/skillIcons/sass.svg" >
                        </div>
                    </div>
                    <div class="ProjetoDesc">
                        <p>Resgate é um projeto que visa ajudar pessoas que estão passando por momentos difíceis, seja por depressão, ansiedade, ou qualquer outro problema psicológico. O projeto foi feito com Next.js e Sass.</p>
                        <button>Visitar</button>
                    </div>
                </div>

                <div class="projeto">
                    <img src="../assets/projetosImgs/Mresgate.png" class="bgProjeto">
                    <div class="Projetoinfo">
                        <h2>Resgate</h2>
                        <div class="techs">
                            <img src="../assets/skillIcons/nextjs.svg" >
                            <img src="../assets/skillIcons/sass.svg" >
                        </div>
                    </div>
                    <div class="ProjetoDesc">
                        <p>Resgate é um projeto que visa ajudar pessoas que estão passando por momentos difíceis, seja por depressão, ansiedade, ou qualquer outro problema psicológico. O projeto foi feito com Next.js e Sass.</p>
                        <button>Visitar</button>
                    </div>
                </div>

            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'Projetos',
}
</script>


<style scoped>

.containerProjetos{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 80vh;
}

.contentProjetos{
    display: flex;
    align-items: center;
    justify-content: center;
    flex-direction: column;
}

.projetos{
    display: flex;
    align-items: center;
    justify-content: center;
    gap: 20px;
    margin-top: 5rem;
}

.projeto{
    width: 30%;
    position: relative;

    transform: scale(1);
    transition: 0.2s ease-out;
}

.projeto img{
    width: 100%;
}

.Projetoinfo{
    position: absolute;
    width: 100%;
    top: 55%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    text-align: center;
}

.projeto:hover{
    transform: scale(1.1);
    transition: 0.5s;

    .bgProjeto{
        filter: brightness(0.2) blur(3px);
        transition: 0.4s easy-in;
    }

    .Projetoinfo {
        opacity: 0;
        transition: 0.4s ease-out;
    }

    .ProjetoDesc{
        opacity: 1;
        transition: 0.8s ease-in;
    }

    z-index: 1;
}


.projeto::before{
    content: '';
    display: block;
    position: absolute;
    width: 100%;
    height: 100%;
    background-color: rgba(0, 0, 0, 0.5);
}

.projeto::after{
    content: '';
    display: block;
    position: absolute;
    width: 100%;
    height: 0.3rem;
    background-image: linear-gradient( to right, #8010A3, #A110A3);
}

.techs{
    margin-right: 10px;
}

.techs img{
    width: 30px;
    height: 30px;
}

.ProjetoDesc{
    position: absolute;
    width: 100%;
    height: 100%;
    top: 50%;
    left: 50%;
    transform: translate(-50%, -50%);
    display: flex;
    flex-direction: column;
    text-align: center;
    opacity: 0;
    justify-content: space-evenly;
}

.ProjetoDesc p{
    font-size: 100%;
    padding: 10px;
}

.ProjetoDesc button{
    padding: 10px;
    border: none;
    cursor: pointer;
    transition: 0.3s ease-in;
    width: 25%;
    height: 2.5rem;
    margin: 0 0 0 65%;
    border-radius: 20px;
    background-color: transparent;
	color: #A110A3;
	border: 1px solid #A110A3;
    font-weight: 600;
    font-family: 'Poppins', sans-serif;
}

.ProjetoDesc button:hover{
    background-image: linear-gradient( to right, #8010A3, #A110A3);
    color: white;
    transform: scale(0.9);
    transition: 0.2s;
}




@media (hover: hover) {

}

@media (max-width: 1024px) {

}

@media (max-width: 800px) {

}
/* media query smartphone */

@media (max-width: 600px) {

}

</style>
