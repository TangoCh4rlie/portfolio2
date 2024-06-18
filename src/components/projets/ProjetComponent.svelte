<script lang="ts">
	import Projet from "./Projet.svelte";

    import serrata from "/src/assets/logo_super_sympa.png";
    import peninsule from "/src/assets/peninsule.png";
    import annuaire from "/src/assets/annuaire.jpg";
    import graph from "/src/assets/graph.jpg";
    import kebab from "/src/assets/kebab_croped.png";
    import panier from "/src/assets/panier.png";

    const projets = [
        {title: "Serrata", description: "Serrata est un projet personnel réalisé avec des amis, c'est un jeu de tappage de drapeaux", img: serrata, link: "https://github.com/SerrataApp"},
        {title: "Projet SAE Penisule", description: "Peninsule à été mon projet de S3, il consistait à créer un site de e-commerce", img: peninsule, link: "https://forge.univ-lyon1.fr/p2201616/sae-s3"},
        {title: "Projet SAE Annuaire", description: "Réalisation d'un programme en C permettant la gestion d'un annuaire à partir d'un fichier CSV contenant des contacts", img: annuaire, link: "https://forge.univ-lyon1.fr/p2201709/c_project_sae"},
        {title: "Projet SAE Parcours de graphe", description: "Ce projet mêlait maths et Java, le but était de faire une application permettant de visualiser et de parcourir un graphe", img: graph, link: "https://forge.univ-lyon1.fr/p2201709/java-sae"},
        {title: "Projet SAE Kebab", description: "Application réalisé en équipe d'un site web static en HTML CSS pour le S1.", img: kebab, link: "https://forge.univ-lyon1.fr/p2201709/sae_kebab"},
        {title: "SupersymPanier", description: "Projet PHP permettant de faire des listes de courses en ligne", img: panier, link: "https://forge.univ-lyon1.fr/p2200578/supersympanier"},
    ]
</script>

<div class="projets">
    <h1 class="title">Projets</h1>
    <div class="parent">
        {#each projets as projet}
            <div class="child">
                <Projet props={projet}/>
            </div>
        {/each}
    </div>
</div>

<style>
    .projets {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .title {
        font-size: 3rem;
        font-weight: bold;
        margin: 1rem;
    }
    .child {
        margin: 1rem;
        background-color: #11181c;
    }
</style>