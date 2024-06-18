<script lang="ts">
    export let props: {title: string, description: string, img: string, link: string};
</script>

<div class="projet">
    <div class="content">
        <h1>{props.title}</h1>
        <p>{props.description}</p>
        <a href="https://github.com/TangoCh4rlie" class="github-button">
            <svg xmlns="http://www.w3.org/2000/svg" width="20" height="20" fill="currentColor" class="bi bi-github" viewBox="0 0 16 16">
                <path d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.54 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.03 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.003 8.003 0 0016 8c0-4.42-3.58-8-8-8z"/>
            </svg>
            Projet GitHub
        </a>
    </div>
    <img src={props.img} alt={props.title} />
</div>

<style>
    .projet {
        margin: 1rem;
        padding: 5rem;
        display: flex;
        position: relative;
        justify-content: space-between;
        align-items: center;
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

    .projet h1 {
        margin: 0;
    }

    .content {
        display: flex;
        flex-direction: column;
        margin: 1rem;
        justify-content: left;
    }

    img {
        justify-content: right;
        width: 200px;
        height: 200px;
        border-radius: 10px;
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

    a {
        display: flex;
        width: 9rem;
        align-items: center;
        justify-content: left;
        text-decoration: none;
        color: #fff;
    }
    .github-button svg {
        margin-right: 10px;
    }
</style>