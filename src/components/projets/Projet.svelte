<script lang="ts">
    export let props: {title: string, description: string, img: string, link: string};
</script>

<div>
    <h1>{props.title}</h1>
    <p>{props.description}</p>
    <img src={props.img} alt={props.title} />
    <a href={props.link}>Lien vers le projet</a>
</div>