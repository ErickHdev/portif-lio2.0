<template>
    <div class="containerContact">
        <div class="contentContact">
            <div class="contatos">
                <div class="circles">
                    <div class="icon">
                        <img class="imgIcon" src="../assets/GitHubIcon.png" />
                    </div>
                    <h4>GitHub</h4>
                    <span>GHub.com/ErickHdev</span>
                </div>

                <div class="circles">
                    <div class="icon">
                        <img class="imgIcon" src="../assets/EmailBox.png" />
                    </div>
                    <h4>Email</h4>
                    <span>erickhds.dev@gmail.com</span>
                </div>
                <div class="circles">
                    <div class="icon">
                        <img class="imgIcon" src="../assets/TelephoneIcon.png" />
                    </div>
                    <h4>Telefone</h4>
                    <span>(83) 98612-5231</span>
                </div>
                <div class="circles">
                    <div class="icon">
                        <img class="imgIcon" src="../assets/LinkedinIcon.png" />
                    </div>
                    <h4>GitHub</h4>
                    <span>GHub.com/ErickHdev</span>
                </div>
            </div>
        </div>
    </div>
</template>


<script>
export default {
    name: 'Contact',
}
</script>


<style scoped>

.containerContact{
    display: flex;
    justify-content: center;
    align-items: center;
    height: 40vh;
}

.contentContact{
    display: flex;
}

.contatos{
    display: flex;
    width: 60vw;
    justify-content: space-around;
}

.circles{
    display: flex;
    align-items: center;
    flex-direction: column;
    height: 18vh;
    width: 20%;
    justify-content: space-around;
    transform: scale(1);
    transition: 0.2s ease-out;

    h4{
        color: #8010A3;
        font-weight: 600;
    }

    
}

.imgContact{
    width: 5rem;
}

.imgIcon{
    width: 60px;
}

.icon{
    border-radius: 100%;
    width: 100px;
    height: 100px;
    background-color: #1f0b35;
    display: flex;
    justify-content: center;
    align-items: center;
}

.circles:hover{
    transform: scale(1.1);
    transition: 0.3s;
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
