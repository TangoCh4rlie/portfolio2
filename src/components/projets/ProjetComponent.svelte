<script lang="ts">
	import Projet from "./Projet.svelte";

    const projets = [
        {title: "Projet SAE Kebab", description: "Application réalisé en équipe d'un site web static en HTML CSS pour le S1.", img: "/src/assets/kebab_croped.png", link: ""},
        {title: "Projet SAE Annuaire", description: "Réalisation d'un programme en C permettant la gestion d'un annuaire à partir d'un fichier CSV contenant des contacts", img: "/src/assets/annuaire.jpg", link: ""},
        {title: "SupersymPanier", description: "Projet PHP permettant de faire des listes de courses en ligne", img: "/src/assets/panier.png", link: ""},
        {title: "Projet SAE Parcours de graphe", description: "Ce projet mêlait maths et Java, le but était de faire une application permettant de visualiser et de parcourir un graphe", img: "/src/assets/graph.jpg", link: ""},
        {title: "Projet SAE Penisule", description: "Peninsule à été mon projet de S3, il consistait à créer un site de e-commerce", img: "/src/assets/peninsule.png", link: ""},
        {title: "Serrata", description: "Serrata est un projet personnel réalisé avec des amis, c'est un jeu de tappage de drapeaux", img: "/src/assets/logo_super_sympa.png", link: ""},
    ]
</script>

<div class="langage">
    <h1 class="title">Technologies</h1>
    <div class="parent">
        {#each projets as projet}
            <div class="child">
                <Projet props={projet}/>
            </div>
        {/each}
    </div>
</div>