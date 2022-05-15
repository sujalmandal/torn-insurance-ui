<script>
	import Header from "./Header.svelte";
	import Body from "./Body.svelte";
	import Footer from "./Footer.svelte";
</script>

<main>
	<Header/>
	<Body/>
	<Footer/>
</main>

<style>
	main {
		top:0px;
    	left:0px;
		text-align: center;
		position: absolute;
		width: 100vw;
		height: 100vh;
        background-color: beige;
		overflow-y: hidden;
	}
</style>