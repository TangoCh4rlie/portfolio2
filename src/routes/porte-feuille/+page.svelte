<script>
	import Header from "../../components/Header.svelte";

    const data = [
        {competence: 'Réaliser', description: 'Je sais développer des solutions informatiques pour des clients, en respectant leurs besoins, en appliquant des principes algorithmiques, et en veillant à la qualité et à la documentation du code, dans le cadre de projets de groupe universitaires (SAE).'},
        {competence: 'Optimiser', description: 'Je sais proposer des applications informatiques optimisées en fonction du temps d’exécution, de la précision et de la consommation de ressources, en modélisant des situations complexes, en utilisant des algorithmes usuels, et en justifiant les choix et les résultats'},
        {competence: 'Administer', description: 'Je sais installer, configurer, maintenir et optimiser des infrastructures, services et réseaux informatiques en sécurisant le système d’information, en appliquant les normes et bonnes pratiques, en offrant une qualité de service optimale et en assurant la continuité d\'activité.'},
        {competence: 'Gérer', description: 'Je sais gérer et exploiter les données d\'une entreprise en respectant les réglementations sur la vie privée, les enjeux économiques et écologiques, et en assurant la qualité des informations pour un bon pilotage.'},
        {competence: 'Conduire', description: 'Je sais organiser et piloter un projet informatique en satisfaisant les besoins des utilisateurs, en respectant les normes et règles juridiques, et en communiquant efficacement avec les acteurs du projet.'},
        {competence: 'Collaborer', description: 'Je sais travailler efficacement au sein d\'une équipe informatique, en accompagnant les évolutions, respectant les contraintes juridiques, et en favorisant une communication collaborative.'},
    ]
</script>

<div class="main-page">
    <Header />
    <div class="page-content">
        {#each data as item}
            <div class="competence">
                <h1>{item.competence}</h1>
                <p>{item.description}</p>
            </div>
        {/each}
    </div>
</div>

<style>
    .main-page {
        background-color: #11181c;
        color: #fff;
        font-family: Inter,sans-serif;
    }

    .page-content {
        position: relative;
        width: 70%;
        margin: 0 auto;
    }

    .competence {
        margin: 2rem;
        position: relative;
        display: flex;
        flex-direction: column;
        align-items: center;
        justify-content: center;
        background-color: #11181c;
        border: 2px solid #ED5432;
        border-radius: 10px;
        box-shadow: 0 0 10px #ED5432;
        padding: 10px 20px;
        color: #fff;
        font-size: 16px;
        font-weight: bold;
        outline: none;
        transition: 0.1s;
        text-decoration: none;
    }

    .competence p {
        text-align: center;
    }
</style>