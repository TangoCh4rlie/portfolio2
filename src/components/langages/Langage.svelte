<script lang="ts">
    export let props: {id: number, name: string, img: string, link: string};
</script>

<a href={props.link}>
    <img src={props.img} alt={props.name} />
    <h2>{props.name}</h2>
</a>

<style>
    a {
        width: 8rem;
        height: 9rem;
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

    a:hover {
        transition: 0.2s;
        box-shadow: 0 0 20px #ED5432;
    }

    img {
        width: 80px;
        height: 80px;
    }
    
    h2 {
        color: #D4D4D4;
        margin: 0;
        margin-top: 15px;
    }
</style>