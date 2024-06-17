<script lang="ts">
	import LangagesGrid from "./langages/LangagesComponent.svelte";
	import ProjetComponent from "./projets/ProjetComponent.svelte";
</script>
<div class="page">
    <!-- <div class="line" /> -->
    <div class="body">
        <div class="top">
            <h1 class="title">
                Elouan Reymond
                <span>
                    TangoCh4rlie
                </span>
            </h1>
        </div>
        <div class="langages">
            <LangagesGrid />
        </div>
        <div class="projet">
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
        justify-content: center;
        align-items: left;
        width: 50%;
    }

    .title {
        display: flex;
        flex-direction: column;
        font-weight: bold;
        font-size: 3rem;
    }

    .title span {
        margin-top: 0.5rem;
        display: flex;
        flex-direction: column;
        background: linear-gradient(#ED5432, #d69533);
        background-clip: border-box;
        -webkit-background-clip: text;
        -webkit-text-fill-color: transparent;
    }

    .langages {
        width: 80%;
        margin: 0 auto;
        display: flex;
        justify-content: center;
    }
</style>