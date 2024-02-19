<template>
    <div class="containerSkills">
        <div class="contentSkills">
            <div class="titleSkills">
                <h1>Skills</h1>
            </div>
            <div class="skills">

                <div class="skill" id="HTML">
                    <img src="../assets/SkillIcons/html5.svg" alt="html5">
                    <h4>HTML</h4>
                </div>

                <div class="skill" id="css">
                    <img src="../assets/SkillIcons/css.svg" alt="html5">
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
    height: 100vh;
}

.titleSkills{
    display: flex;
    align-items: center;
    justify-content: center;
}

.contentSkills {
    display: flex;
    flex-direction: column;
    align-items: center;
    justify-content: space-between;
    width: 65rem;
    height: 48rem;
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
    justify-content: space-between;
    background-color: #1f0b35;
    padding: 1rem;
    border-radius: 15px;
    box-shadow: 0 0 10px rgba(0, 0, 0, 0.5);
    transition: 0.3s;
    width: 14.2rem;
    height: 12rem;
}

.skill:hover{
    transform: scale(1.1)
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

}

</style>
