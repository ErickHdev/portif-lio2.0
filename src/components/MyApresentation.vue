<template>
    <div class="myApresentation">
        <div class="apresentationText">
						<p>Hello 😆, I'm</p>

            <h1>Erick Henrique</h1>

						<p class="devFront">Desenvolvedor Frontend 🖥️</p>

						<div class="btnsContact">
							<a href="https://www.linkedin.com/in/erick-hdev" target="_blank">
								<button class="buttonContact">Contate-me</button>
							</a>
							<a href="https://www.github.com/erickHdev" target="_blank">
								<button class="buttonCV">CV</button>
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
		height: 100vh;
		color: white;
		margin-inline: 10%;
		background-image: linear-gradient( to right, #0E041D, #150323);
}

.apresentationText{
		display: flex;
		flex-direction: column;
		height: 450px;

		p {
			font-size: 3rem;
			margin-left: 3px;
		}

		h1{
			font-size: 6rem;
			line-height: 4rem;
		}
}

.bgImage{
		border-radius: 53% 83% 84% 19% / 79% 57% 77% 57%  ;
		background-image: linear-gradient( to top right, #9610A3, #A110A3);
		box-shadow: 0 0 60px 20px #A110A3;
}

.btnsContact{
		display: flex;
		justify-content: space-between;
		width: 450px;
		margin-top: 20px;
		margin-left: 3px;
		margin-bottom: 20px;
		margin: 0;
}

.buttonContact{
		width: 200px;
		height: 40px;
		background-image: linear-gradient( to right, #8010A3, #A110A3);;
		color: white;
		border: none;
		text-align: center;
		text-decoration: none;
		font-size: 1.2rem;
		border-radius: 15px;
}

.buttonCV{
		width: 200px;
		height: 40px;
		background-color: transparent;
		color: #A110A3;
		border: 1px solid #A110A3;
		text-align: center;
		text-decoration: none;
		font-size: 1.2rem;
		border-radius: 15px;

}


@media (hover: hover) {

}

/* media query smartphone */

@media (max-width: 1024px) {
	.myApresentation{
		flex-direction: column;
		justify-content: center;
		align-items: center;
		height: 100vh;
		width: 100vw;
		margin: 0;
	}

	.apresentationText{
		text-align: center;
		height: 15rem;
		padding: 0;


		p {
			text-align: left;
			font-size: 0.9rem;
			margin: 0;
			margin-left: 3px;
			line-height: 2rem;
		}

		h1{
			font-size: 2.8rem;
			line-height: 2rem;
			margin: 0;
		}

		.devFront{
			font-size: 1.3rem;
			margin: 0;
			margin-left: 3px;
			line-height: 3.3rem;
		}
	}

	.bgImage{
		width: 70vw;
		height: 80vw;
		display: flex;
		justify-content: center;
		align-items: center;
		border-radius: 53% 83% 84% 19% / 79% 57% 77% 57%  ;
		background-image: linear-gradient( to top right, #9610A3, #A110A3);
		box-shadow: 0 0 60px 20px #A110A3;

		img{
			width: 70vw;
			height: 70vw;
		}
	}

	.btnsContact{
		display: flex;
		justify-content: space-between;
		align-items: center;
		width: 95%;
		margin-top: 20px;
		margin-left: 3px;
		margin: 0;
	}

	.buttonContact{
		width: 130px;
		height: 35px;
		background-image: linear-gradient( to right, #8010A3, #A110A3);;
		color: white;
		border: none;
		text-align: center;
		text-decoration: none;
		font-size: 1rem;
		border-radius: 15px;
		margin-bottom: 10px;
		margin: 0;
	}

	.buttonCV{
		width: 130px;
		height: 35px;
		background-color: transparent;
		color: #A110A3;
		border: 1px solid #A110A3;
		text-align: center;
		text-decoration: none;
		font-size: 1rem;
		border-radius: 15px;
	}
}

</style>
