<template>
    <div class="containerSkills">
        <div class="contentSkills">
            <div class="titleSkills">
                <span><img src="../assets/code-icon.svg">Skills</span>
                <h1>Habilidades</h1>
            </div>
            <div class="skills">

                <div class="skill" id="HTML">
                    <img src="../assets/SkillIcons/html5.svg" alt="html5">
                    <h4>HTML</h4>
                </div>

                <div class="skill" id="css">
                    <img src="../assets/skillIcons/css.svg" alt="html5">
                    <h4>CSS</h4>
                </div>

                <div class="skill" id="js">
                    <img src="../assets/SkillIcons/JavaScript.svg" alt="html5">
                    <h4>JavaScript</h4>
                </div>

                <div class="skill" >
                    <img src="../assets/SkillIcons/typescript.png" alt="html5">
                    <h4>TypeScript</h4>
                </div>

                <div class="skill" >
                    <img src="../assets/SkillIcons/nextjs.svg" alt="html5">
                    <h4>Nextjs</h4>
                </div>

                <div class="skill" >
                    <img src="../assets/SkillIcons/react.svg" alt="html5">
                    <h4>ReactJs</h4>
                </div>

                <div class="skill" >
                    <img src="../assets/SkillIcons/vuejs.svg" alt="html5">
                    <h4>VueJs</h4>
                </div>
                
                <div class="skill" >
                    <img src="../assets/SkillIcons/git.svg" alt="html5">
                    <h4>Git</h4>
                </div>

                <div class="skill" >
                    <img src="../assets/SkillIcons/bootstrap.svg" alt="html5">
                    <h4>Bootstrap</h4>
                </div>

                <div class="skill" >
                    <img src="../assets/SkillIcons/sass.svg" alt="html5">
                    <h4>SASS</h4>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'Skills',
}
</script>


<style scoped>

.containerSkills{
    display: flex;
    align-items: center;
    justify-content: center;
    height: 110vh;
}

.titleSkills{
    display: flex;
    align-items: center;
    justify-content: center;
}

.titleSkills h1{
    font-size: 3.5rem;
    font-weight: 800;
    color: #A110A3;
    margin-bottom: 2rem;
}

.titleSkills span{
    position: absolute;
    font-size: 5rem;
    font-weight: 800;
    color: #A110A3;
    opacity: 0.2;
    z-index: -1;
    margin-bottom: 6rem;
}

.titleSkills img{
    width: 100px;
    margin-right: 1rem;
    transform: rotate(-30deg);
    filter: invert(16%) sepia(76%) saturate(4792%) hue-rotate(291deg) brightness(78%) contrast(100%);
}

.contentSkills {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    width: 65rem;
    height: 50rem;
}

.skills{
    display: grid;
    grid-template-columns: repeat(4, 1fr);
    gap: 2rem;
}

.skill{
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: center;
    background-color: #1f0b35;
    padding: 1rem;
    border-radius: 15px;

    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
    transition: 0.3s;
    width: 14.2rem;
    height: 12rem;

    position: relative;
    overflow: hidden;

    img, h4{
        z-index: 1;
    }

    h4{
        margin-top: 1rem;
        font-family: montserrat;
    }
}

.skill::before{
    content: "";
    position: absolute;
    width: 110px;
    height: 150%;
    background-color: #A110A3;
    box-shadow: 0 0 20px 20px #A110A3;
    animation: skillAnimation 8s linear infinite;
}

@keyframes skillAnimation {
    100% {
        transform: rotate(360deg);
    }
}

.skill::after{
    content: '';
    position: absolute;
    background-color: #1f0b35;
    inset: 5px;
    border-radius: inherit;

}

.skill:hover{
    transform: scale(1.02);
}

.skill img{
    width: 100px;
    height: 100px;
}


@media (hover: hover) {

}

@media (max-width: 1024px) {

}

@media (max-width: 800px) {

}
/* media query smartphone */

@media (max-width: 600px) {
    .containerSkills{
        display: flex;
        align-items: center;
        justify-content: center;
        height: 150vh;
    }

    .skills {
        grid-template-columns: repeat(2, 1fr);
    }

    .skill{ 
        width: 8rem;
        height: 8rem;

        img{
            width: 55px;
            height: 55px;
        }
    }

    .skill::before{
        content: "";
        position: absolute;
        width: 20px;
        height: 150%;
        background-color: #A110A3;
        box-shadow: 0 0 20px 20px #A110A3;
        animation: skillAnimation 8s linear infinite;
    }

    .titleSkills h1{
        font-size: 2.25rem;
        font-weight: 800;
        color: #A110A3;
        margin-bottom: 2rem;
    }

    .titleSkills span{
        position: absolute;
        font-size: 3rem;
        font-weight: 800;
        color: #A110A3;
        opacity: 0.2;
        z-index: -1;
        margin-bottom: 5rem;
    }

    .titleSkills img{
        width: 80px;
        margin-right: 1rem;
    }
}

</style>
