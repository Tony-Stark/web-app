<script>
	import Todos from './components/Todos.svelte'
	let name = "Yossi";
	let todos = [
		{id : 1, name : "create first mission", completed : true},
		{id : 2, name : "create second mission", completed : true},
		{id : 3, name : "create third mission", completed : true},
		{id : 4, name : "create fourth mission", completed : true},
		{id : 5, name : "create fifth mission", completed : false},
		{id : 6, name : "create sixth mission", completed : false},
		{id : 7, name : "create seventh mission", completed : false},
	];
</script>

<Todos {todos} />

<main>
	<h1>Hello {name}!</h1>
	<p>Visit the <a href="https://svelte.dev/tutorial">Svelte tutorial</a> to learn how to build Svelte apps.</p>
</main>

<style>
	main {
		text-align: center;
		padding: 1em;
		max-width: 240px;
		margin: 0 auto;
	}

	h1 {
		color: #ff3e00;
		text-transform: uppercase;
		font-size: 4em;
		font-weight: 100;
	}

	@media (min-width: 640px) {
		main {
			max-width: none;
		}
	}
</style>
