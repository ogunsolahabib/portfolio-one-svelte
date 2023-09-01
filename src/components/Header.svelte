<script lang="ts">
	import { themeStore } from 'svelte-theme-switch';
</script>

<header>
	<nav class="main-nav">
		<div class="brand-logo">
			<a href="/">
				<h1>&lt;h/&gt;</h1>
			</a>
		</div>
		<div class="right">
			<button
				on:click={() => $themeStore.setTheme($themeStore.theme === 'light' ? 'dark' : 'light')}
			>
				Switch Theme
			</button>
			<a
				target="_blank"
				rel="noopener noreferrer"
				href="https://docs.google.com/document/d/e/2PACX-1vSrcUD2WThZGZTSAN1bRfNMy1Zp5ZZEupuMY_xL6X0oc3A3dD5IuYWgq9ftqEVwx4si8zRpOJjCrfWd/pub"
			>
				<button class="btn btn-primary">RESUME</button>
			</a>
		</div>
	</nav>
</header>

<style>
	.brand-logo h1 {
		font-size: 5rem;
		vertical-align: middle;
		text-align: center;
		font-family: 'Dancing Script', cursive, sans-serif;
	}

	.main-nav {
		display: flex;
		align-items: center;
		justify-content: space-between;
	}
</style>
