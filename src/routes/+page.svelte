<script>
	import { message } from '@tauri-apps/api/dialog';

	function hello() {
		  message('Svelte in Tauri', 'Message');
	}
</script>

<div class="container">
	<h1>SvelteKit ❤️️ Tauri</h1>
	<h2>beautiful world</h2>
    <button on:click={hello}>hello</button>
</div>

<style>
	.container {
		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		height: 100vh;
	}
	h1 {
		color: white;
	}
	h2 {
		color: white;
	}
    button {
        background-color: rgb(255, 107, 107);
        color: white;
        border: none;
        padding: 10px 20px;
        border-radius: 15px;
        font-size: 24px;
        cursor: pointer;
    }
	:global(body) {
		background: black;
        overflow: hidden;
	}
</style>
