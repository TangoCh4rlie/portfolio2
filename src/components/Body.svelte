<script lang="ts">
	import LangagesGrid from './langages/LangagesComponent.svelte';
	import ProjetComponent from './projets/ProjetComponent.svelte';
</script>

<div class="page">
	<!-- <div class="line" /> -->
	<div class="body">
		<div class="top">
			<h1 class="title">
				Elouan Reymond
				<span> TangoCh4rlie </span>
			</h1>
			<div class="pf-cpt">
				<a href="/porte-feuille" class="github-button">
					Porte-feuille de compétences
				</a>
			</div>
		</div>
		<div class="langages" id="langages">
			<LangagesGrid />
		</div>
		<div class="projets" id="projets">
			<ProjetComponent />
		</div>
	</div>
</div>

<style>
	.page {
		display: flex;
		width: 70%;
		margin: 0 auto;
	}

	/* .line {
        width: 1px;
        height: 1000px;
        background-color: #ED5432;
    } */

	.body {
		width: 100%;
		display: flex;
		flex-direction: column;
	}

	.top {
		display: flex;
		align-items: center;
		width: 100%;
	}

	.pf-cpt {
		width: 50%;
		display: flex;
		justify-content: center;
	}

	.pf-cpt a {
		text-decoration: none;
		width: 14rem;
	}

	.title {
		display: flex;
		flex-direction: column;
		font-weight: bold;
		font-size: 3rem;
		width: 50%;
	}

	.title span {
		margin-top: 0.5rem;
		display: flex;
		flex-direction: column;
		background: linear-gradient(#ed5432, #d69533);
		background-clip: border-box;
		-webkit-background-clip: text;
		-webkit-text-fill-color: transparent;
	}

	.langages {
		width: 80%;
		margin: 0 auto;
		display: flex;
		justify-content: center;
		margin-top: 5rem;
		margin-bottom: 5rem;
	}

	.projets {
		width: 80%;
		margin: 0 auto;
		display: flex;
		justify-content: center;
	}

	.github-button {
        display: flex;
        align-items: center;
        background-color: transparent;
        border: 2px solid #006cc5;
        border-radius: 10px;
        box-shadow: 0 0 10px #006cc5;
        padding: 10px 20px;
        color: #fff;
        font-size: 16px;
        font-weight: bold;
        outline: none;
        transition: 0.1s;
    }
    .github-button:hover {
        transition: 0.2s;
        box-shadow: 0 0 20px #006cc5;
    }
</style>
