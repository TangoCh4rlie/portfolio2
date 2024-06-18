<script lang="ts">
    import {fade} from "svelte/transition"
	import Header from "../components/Header.svelte";
    import Body from "../components/Body.svelte";
    let m: any = null;
	function mousemove(event: any) {
		let r = event.currentTarget.getBoundingClientRect();
		m = {x:event.clientX-r.left, y:event.clientY-r.top}
	}
	function mouseleave(event: any) {
		m = null;
	}
</script>

<!-- svelte-ignore a11y-no-static-element-interactions -->
<div class="main-page" on:mousemove={mousemove} on:mouseleave={mouseleave}>
    {#if m}
		<div transition:fade  class="blob" style:transform="translate({m.x}px, {m.y}px)"></div>
	{/if}
    <Header />
    <Body />
</div>

<style>
    .main-page {
        background-color: #11181c;
        background-color: #11181c;
        color: #fff;
        font-family: Inter,sans-serif;
        position: relative;
    }
    .blob {
        filter: blur(100px);
        position: absolute;
        top: -150px;
        left: -150px;
        width: 300px;
        height: 300px;
        /* top: -50px;
        left: -50px;
        width: 150px;
        height: 150px; */
        border-radius: 50%;
        background: rgba(121, 85, 51, 0.3);
        pointer-events:none;
    }
</style>
