<script>
	import Header from "./Header.svelte";
	let name = 'Wally';
	function toggleTheme() {
		document.body.classList.toggle('light');
		document.body.classList.toggle('dark');
	}
</script>

<svelte:head>
	<title>Welcome to FreeApks</title>
	<meta name="description" content="A page about me" />
</svelte:head>

<div id="root">
	<Header />
	<h1>Hello {name}</h1>
	<button on:click={toggleTheme}>Click me</button>
</div>

<style>
:global(body) {
	font-family: sans-serif;
	background-color: var(--primary);
	color: var(--text);
	padding: 0;
	margin: 0;
}

:global(.light) {
	--primary: #606c38;
	--secondary: #283618;
	--buttons: #dda15e;
	--text: #fefae0;
	--highlight: #bc6c25;
}

:global(.dark) {
	--primary: #a3b18a;
	--secondary: #588157
	--text: #dad7cd;
	--buttons: #344e41;
	--highlight: #3a5a40;
}

</style>
