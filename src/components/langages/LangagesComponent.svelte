<script>
	import Langage from "./Langage.svelte";
    import js from "/src/assets/js.png";
    import ts from "/src/assets/ts.png";
    import python from "/src/assets/python.png";
    import c from "/src/assets/c.png";
    import java from "/src/assets/java.png";

    const langages = [
        {id: 1, name: "JavaScript", img: js, link: "https://developer.mozilla.org/fr/docs/Web/JavaScript"},
        {id: 2, name: "TypeScript", img: ts, link: "https://www.typescriptlang.org/"},
        {id: 3, name: "Python", img: python, link: "https://www.python.org/"},
        {id: 4, name: "C", img: c, link: "https://fr.wikipedia.org/wiki/C_(langage)"},
        {id: 5, name: "Java", img: java, link: 'https://fr.wikipedia.org/wiki/Java_(langage)'},
    ]

</script>

<div class="langage">
    <h1 class="title">Technologies</h1>
    <div class="parent">
        {#each langages as langage}
            <div class="child">
                <Langage props={langage}/>
            </div>
        {/each}
    </div>
</div>

<style>
    .langage {
        display: flex;
        flex-direction: column;
        justify-content: center;
    }
    .title {
        font-size: 3rem;
        font-weight: bold;
        margin-top: 2rem;
        margin-bottom: 2rem;
    }
    .parent {
        display: flex;
        flex-wrap: wrap;
    }
    .child {
        margin: 1rem;
    }

    /* div:nth-child(2n) {

    } */
</style>
