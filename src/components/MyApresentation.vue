<template>
    <div class="myApresentation">
        <div class="apresentationText">
			<p>Hello 😆, I'm</p>
            <h1>Erick Henrique</h1>
			<p class="devFront">Desenvolvedor Frontend 🖥️</p>
			

			<div class="containerBtns">
				<a href="https://www.linkedin.com/in/erick-hdev" target="_blank">
					<button class="buttonContact btnW">Contate-me</button>
				</a>
				<a href="https://www.github.com/erickHdev" target="_blank">
					<button class="buttonCV btnW">CV</button>
				</a>
			</div>
        </div>
        <div class="bgImage">
			<img src="@/assets/euDev.png" alt="Logo" />
        </div>
    </div>

</template>


<script>
export default {
    name: 'ApresentationApp',
    
}
</script>


<style scoped>
.myApresentation{
	display: flex;
	align-items: center;
	justify-content: space-between;
	height: 85vh;
	color: white;
	margin-inline: 18%;
	padding-top: 10vh;
}

.apresentationText {
	display: flex;
	flex-direction: column;
	height: 15vw;

	p {
		font-size: 1.5vw;
		margin: 0;
		margin-left: 2px;
	}

	h1 {
		font-size: 3vw;
		line-height: 2.5vw;
		font-weight: 800;
	}
}

.containerBtns {
	display: flex;
	justify-content: space-between;
	width: 15vw;
	margin-left: 4px;
}

.btnW {
	width: 6vw;
	height: 30px;
	text-align: center;
	text-decoration: none;
	border-radius: 15px;
	font-size: 0.8vw;
}

.buttonContact {
	background-image: linear-gradient( to right, #8010A3, #A110A3);
	color: white;
	border: none;
}

.buttonCV {
	background-color: transparent;
	color: #A110A3;
	border: 1px solid #A110A3;
}

.bgImage {
	border-radius: 53% 83% 84% 19% / 79% 57% 77% 57%;
	background-image: linear-gradient( to top right, #9610A3, #A110A3);
	box-shadow: 0 0 60px 20px #A110A3;

	img {
		width: 20vw;
		height: 20vw;
	}
}

@media (hover: hover) {

}

@media (max-width: 1600px) {
	.myApresentation {
		margin-inline: 18%;
	}

	.apresentationText{
		p {	
			font-size: 2.5vw;
			margin-left: 2px;
		}
		h1 {
			font-size: 4vw;
			line-height: 3vw;
		}
	}
}

@media (max-width: 1300px) {
	.myApresentation {
		margin-inline: 15%;
		height: 70vh;
	}

	.apresentationText{
		p{	
			font-size: 2.5vw;
			margin-left: 2px;
		}
		h1 {
			font-size: 4vw;
			line-height: 3vw;
		}
	}

	.containerBtns {
		width: 22vw;
	}
	.btnW {
		width: 9vw;
		height: 30px;
		text-align: center;
		font-size: 1.2vw;
	}
}

/* media query low resolution */

@media (max-width: 1024px) {
	.myApresentation {
		height: 60vh;
	}

	.apresentationText{
		p{	
			font-size: 2.5vw;
			margin-left: 2px;
		}
		h1 {
			font-size: 4.5vw;
			line-height: 3vw;
		}
	}

	.containerBtns {
		width: 22vw;
	}

	.btnW {
		width: 9vw;
		height: 25px;
		text-align: center;
		font-size: 1.2vw;
	}
}

/* media query smartphone */

@media (max-width: 800px) {
	.myApresentation {
		height: 70vh;
	}
	
}


@media (max-width: 660px) {
	.myApresentation {
		flex-direction: column;
		justify-content: space-between;
		height: 100vh;
		padding-block: 15vh;
	}

	.apresentationText {
		p {
			font-size: 5vw;
			margin-left: 2px;
		}

		h1 {
			font-size: 10+vw;
			line-height: 4.5vh;
		}
	}

	.containerBtns {
		display: flex;
		justify-content: space-between;
		align-items: center;
		width: 60vw;
		margin-top: 10px;
		margin-left: 2px;
	}


	.btnW {
		width: 28vw;
		height: 30px;
		text-align: center;
		text-decoration: none;
		border-radius: 15px;
		font-size: 2vh;
	}

	.buttonContact {
		background-image: linear-gradient( to right, #8010A3, #A110A3);
		color: white;
		border: none;
	}

	.buttonCV {
		background-color: transparent;
		color: #A110A3;
		border: 1px solid #A110A3;
	}

	.bgImage {
		display: flex;
		justify-content: center;
		align-items: center;
		margin: 0;

		img {
			width: 70vw;
			height: 70vw;
		}
	}
}

</style>
