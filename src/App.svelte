<script>
  let list = [
		{id:0, content:'Task #0', done: false},
		{id:1, content:'Task #1', done: false},
		{id:2, content:'Task #2', done: true},
		{id:3, content:'Task #3', done: false}
	]
</script>

<ul>
	{#each list as item}
	<li>
		<p>{item.id}</p>
		<p>{item.content}</p>
		<p>{item.done}</p>
	</li>
	{/each}
</ul>

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
